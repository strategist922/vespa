# Copyright 2017 Yahoo Holdings. Licensed under the terms of the Apache 2.0 license. See LICENSE in the project root.
vespa_add_executable(searchcore_documentbucketmover_test_app TEST
    SOURCES
    documentbucketmover_test.cpp
    DEPENDS
    searchcore_test
    searchcore_server
    searchcore_persistenceengine
    searchcore_feedoperation
    searchcore_matching
    searchcore_attribute
    searchcore_documentmetastore
    searchcore_bucketdb
    searchcore_pcommon
    searchcore_grouping
    searchcore_util
    searchcore_fconfig
)
vespa_add_test(NAME searchcore_documentbucketmover_test_app COMMAND searchcore_documentbucketmover_test_app)
