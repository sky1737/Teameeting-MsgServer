noinst_LIBRARIES=libMSCommon.a

AM_CFLAGS=-g -std=c++11 -Wall -fPIC -D__PTHREADS__ -D__PTHREADS_MUTEXES__

AM_CPPFLAGS=$(AM_CFLAGS)

AM_CPPFLAGS+= -I$(top_srcdir)/../ \
		   -I$(top_srcdir)/MSCommon/MSBase/ \
		   -I$(top_srcdir)/MSCommon/MSCommon/ \
		   -I$(top_srcdir)/MSCommon/MSHttp/ \
		   -I$(top_srcdir)/MSCommon/MSThirdParty/ \
		   -I$(top_srcdir)/MSCommon/MSThirdParty/autoref/ \
		   -I$(top_srcdir)/MSCommon/MSThirdParty/hiredis/ \
		   -I$(top_srcdir)/MSCommon/MSThirdParty/libhttp/ \
		   -I$(top_srcdir)/MSCommon/MSThirdParty/RTComm/ \
		   -I$(top_srcdir)/MSCommon/MSThirdParty/zkclient/common/include \
		   -I$(top_srcdir)/MSCommon/MSThirdParty/zkclient/efnfw \
		   -I$(top_srcdir)/MSCommon/MSThirdParty/rtklog/

noinst_HEADERS=$(top_srcdir)/MSCommon/PlatformHeader.h \
			   $(top_srcdir)/MSCommon/revision.h \
			   $(top_srcdir)/MSCommon/sigslot.h \
			   $(top_srcdir)/MSCommon/config_parser.h \
			   $(top_srcdir)/MSCommon/ProtoCommon.h

libMSCommon_a_SOURCES= \
				$(top_srcdir)/proto/common_msg.pb.cc \
				$(top_srcdir)/proto/entity_msg.pb.cc \
				$(top_srcdir)/proto/entity_msg_type.pb.cc \
				$(top_srcdir)/proto/sys_msg.pb.cc \
				$(top_srcdir)/proto/sys_msg_type.pb.cc \
				$(top_srcdir)/proto/storage_msg.pb.cc \
				$(top_srcdir)/proto/storage_msg_type.pb.cc \
				$(top_srcdir)/MSCommon/sigslot.cc \
				$(top_srcdir)/MSCommon/config_parser.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTTcp.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTTcpNoTimeout.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTDispatch.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTEventLooper.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTEventTimer.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTJSBuffer.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTUtils.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTTransfer.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTLstorage.cpp \
				$(top_srcdir)/MSCommon/MSBase/RTZKClient.cpp \
				$(top_srcdir)/MSCommon/MSBase/MsConfigParser.cpp \
				$(top_srcdir)/MSCommon/MSHttp/RTHttp.cpp \
				$(top_srcdir)/MSCommon/MSHttp/RTConnHttp.cpp \
				$(top_srcdir)/MSCommon/MSHttp/RTHttpSender.cpp \
				$(top_srcdir)/MSCommon/MSHttp/RTHttpSvrConn.cpp

