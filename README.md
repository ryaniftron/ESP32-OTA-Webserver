Changes from factory espidf menuconfig
1. Enable OTA parition : Partition Table -> PARTITION_TABLE_TWO_OTA =y
1. Allow http OTA : component config-> ESP HTTPS Ota -> OTA_ALLOW_HTTP =y
1. Increase flash size to 4MB: Partitions defined in '/home/ryan/esp/esp-idf/components/partition_table/partitions_two_ota.csv' occupy 3.1MB of flash (3211264 bytes) which does not fit in configured flash size 2MB. Change the flash size in menuconfig under the 'Serial Flasher Config' menu.
 
