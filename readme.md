nRF52
=====

To test the BLE UART, download and open nRF UART:

https://play.google.com/store/apps/details?id=com.nordicsemi.nrfUARTv2

And execute these instructions from the repo:

    cd examples/dfu/bootloader/pca10036/dual_bank_ble_s132/armgcc
    make flash_all

    stty -icanon 0 -F /dev/ttyACM0 38400
    echo "Hello, World!" > /dev/ttyACM0
    cat /dev/ttyACM0

...you should see something in your app. You can also reply, it should appear in the terminal.


TODO: add tools downloads.

