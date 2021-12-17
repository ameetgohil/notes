## PCIe

Remove device:
`sudo sh -c "echo 1 > /sys/bus/pci/devices/0000\:07\:00.0/remove"`

rescan:
`sudo sh -c "echo 1 > /sys/bus/pci/rescan "`

enable:
`sudo setpci -s 07:00.0 COMMAND=0x2`

status:
`sudo lspci -vv`
