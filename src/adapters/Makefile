binary_name			:= adapters.so
type				:= lib

include_folders			:= inc ../domain/inc ../application/inc \
                                   ../../lib/spdlog/install/include ../../lib/yaml/install/include \
                                   ../../lib/json/install/include ../../lib/pqxx/install/include \
                                   ../../lib/restbed/install/include ../../lib/cpputest/install/include
library_folders			:= ../domain/build/debug/lib ../application/build/debug/lib \
                                   ../../lib/spdlog/install/lib ../../lib/yaml/install/lib ../../lib/pq/install/lib ../../lib/pqxx/install/lib \
                                   ../../lib/restbed/install/library ../../lib/cpputest/install/lib
libs_to_link			:=
test_libs_to_link		:= stdc++ pthread :domain.so :application.so \
                                   :libspdlog.a :libyaml-cpp.a :libpqxx.so :libpq.so :librestbed.so \
                                   :libCppUTest.a :libCppUTestExt.a

base_source_folders		:= src src/repositories src/controllers src/drivers/logger src/drivers/persistence src/drivers/http src/drivers/config
test_source_folders		:= test

include ../module.mk
