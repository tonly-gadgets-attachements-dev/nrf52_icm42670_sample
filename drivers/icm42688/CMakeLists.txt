# SPDX-License-Identifier: Apache-2.0
include_directories(.)
target_sources(app PRIVATE icm42688.c icm42688_spi.c)
target_sources_ifdef(CONFIG_ICM42688_TRIGGER app PRIVATE icm42688_trigger.c)