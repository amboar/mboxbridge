ACLOCAL_AMFLAGS = -I m4
sbin_PROGRAMS = mboxd mboxctl

mboxd_SOURCES = mboxd.c common.c mboxd_dbus.c mboxd_flash.c mboxd_lpc.c mboxd_msg.c mboxd_windows.c mtd.c
mboxd_CFLAGS = $(LIBSYSTEMD_CFLAGS)
mboxd_LDFLAGS = $(LIBSYSTEMD_LIBS)

mboxctl_SOURCES = mboxctl.c
mboxctl_LDFLAGS = $(LIBSYSTEMD_LIBS)
mboxctl_CFLAGS = $(LIBSYSTEMD_CFLAGS)

@CODE_COVERAGE_RULES@
test_copy_flash_SOURCES = test/copy_flash.c mboxd_flash.c common.c mtd.c test/tmpf.c
test_copy_flash_LIBS = $(CODE_COVERAGE_LIBS)
test_copy_flash_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_copy_flash_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_erase_flash_SOURCES = test/erase_flash.c mboxd_flash.c common.c test/tmpf.c
test_erase_flash_LIBS = $(CODE_COVERAGE_LIBS)
test_erase_flash_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_erase_flash_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_write_flash_SOURCES = test/write_flash.c mboxd_flash.c common.c test/tmpf.c
test_write_flash_LIBS = $(CODE_COVERAGE_LIBS)
test_write_flash_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_write_flash_CFLAGS = $(CODE_COVERAGE_CFLAGS)

TEST_MBOX_SRCS = mboxd_msg.c mboxd_windows.c mboxd_lpc.c mboxd_flash.c common.c
TEST_MOCK_SRCS = test/tmpf.c test/mbox.c test/system.c

test_get_mbox_info_v2_SOURCES = test/get_mbox_info_v2.c \
				$(TEST_MBOX_SRCS) \
				$(TEST_MOCK_SRCS)
test_get_mbox_info_v2_LIBS = $(CODE_COVERAGE_LIBS)
test_get_mbox_info_v2_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_get_mbox_info_v2_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_reset_state_SOURCES = test/reset_state.c \
			   $(TEST_MBOX_SRCS) \
			   $(TEST_MOCK_SRCS)
test_reset_state_LIBS = $(CODE_COVERAGE_LIBS)
test_reset_state_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_reset_state_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_get_flash_info_v2_SOURCES = test/get_flash_info_v2.c \
				 $(TEST_MBOX_SRCS) \
				 $(TEST_MOCK_SRCS)
test_get_flash_info_v2_LIBS = $(CODE_COVERAGE_LIBS)
test_get_flash_info_v2_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_get_flash_info_v2_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_create_read_window_v2_SOURCES = test/create_read_window_v2.c \
				     $(TEST_MBOX_SRCS) \
				     $(TEST_MOCK_SRCS)
test_create_read_window_v2_LIBS = $(CODE_COVERAGE_LIBS)
test_create_read_window_v2_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_create_read_window_v2_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_create_write_window_v2_SOURCES = test/create_write_window_v2.c \
				      $(TEST_MBOX_SRCS) \
				      $(TEST_MOCK_SRCS)
test_create_write_window_v2_LIBS = $(CODE_COVERAGE_LIBS)
test_create_write_window_v2_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_create_write_window_v2_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_close_window_v2_SOURCES = test/close_window_v2.c \
			       $(TEST_MBOX_SRCS) \
			       $(TEST_MOCK_SRCS)
test_close_window_v2_LIBS = $(CODE_COVERAGE_LIBS)
test_close_window_v2_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_close_window_v2_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_mark_write_dirty_v2_SOURCES = test/mark_write_dirty_v2.c \
				   $(TEST_MBOX_SRCS) \
				   $(TEST_MOCK_SRCS)
test_mark_write_dirty_v2_LIBS = $(CODE_COVERAGE_LIBS)
test_mark_write_dirty_v2_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_mark_write_dirty_v2_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_write_flush_v2_SOURCES = test/write_flush_v2.c \
			      $(TEST_MBOX_SRCS) \
			      $(TEST_MOCK_SRCS)
test_write_flush_v2_LIBS = $(CODE_COVERAGE_LIBS)
test_write_flush_v2_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_write_flush_v2_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_mark_write_erased_v2_SOURCES = test/mark_write_erased_v2.c \
				    $(TEST_MBOX_SRCS) \
				    $(TEST_MOCK_SRCS)
test_mark_write_erased_v2_LIBS = $(CODE_COVERAGE_LIBS)
test_mark_write_erased_v2_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_mark_write_erased_v2_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_bmc_event_ack_v2_SOURCES = test/bmc_event_ack_v2.c \
				$(TEST_MBOX_SRCS) \
				$(TEST_MOCK_SRCS)
test_bmc_event_ack_v2_LIBS = $(CODE_COVERAGE_LIBS)
test_bmc_event_ack_v2_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_bmc_event_ack_v2_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_create_oversize_window_SOURCES = test/create_oversize_window.c \
				      $(TEST_MBOX_OBJS) \
				      $(TEST_MOCK_OBJS)
test_create_oversize_window_LIBS = $(CODE_COVERAGE_LIBS)
test_create_oversize_window_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_create_oversize_window_CFLAGS = $(CODE_COVERAGE_CFLAGS)

test_create_zero_size_window_SOURCES = test/create_zero_size_window.c \
				       $(TEST_MBOX_OBJS) \
				       $(TEST_MOCK_OBJS)
test_create_zero_size_window_LIBS = $(CODE_COVERAGE_LIBS)
test_create_zero_size_window_CPPFLAGS = $(CODE_COVERAGE_CPPFLAGS)
test_create_zero_size_window_CFLAGS = $(CODE_COVERAGE_CFLAGS)

check_PROGRAMS = test/copy_flash \
		 test/erase_flash \
		 test/write_flash \
		 test/reset_state \
		 test/get_mbox_info_v2 \
		 test/get_flash_info_v2 \
		 test/create_read_window_v2 \
		 test/create_write_window_v2 \
		 test/close_window_v2 \
		 test/mark_write_dirty_v2 \
		 test/write_flush_v2 \
		 test/mark_write_erased_v2 \
		 test/bmc_event_ack_v2 \
		 test/create_oversize_window \
		 test/create_zero_size_window

TESTS = $(check_PROGRAMS)
