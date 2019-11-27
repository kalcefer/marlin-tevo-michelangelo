# marlin-tevo-michelangelo
This is marlin 1.1.9 configured for Tevo Michelangelo 3D printer in stock configuration.

NOTE: Fix for Tevo Michelangelo's low contrast LCD issue.

1. Locate a u8glib library file <your arduino libraries>\U8glib\src\clib\u8g_dev_uc1701_mini12864.c
2. Find contrast field in the init sequence. Default value is 0x027.
3. This is six bit variable. So it has 0x000 - 0x03F range. Looks like 0x030 produces good results.  
