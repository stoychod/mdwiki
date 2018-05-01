### From the command line

#### For FAT32:
```bash
sudo mlabel -i /dev/sdc1 ::"my_label"
```

#### For NTFS:
```bash
sudo ntfslabel /dev/sdc1 my_label
```

#### For exFAT:
```bash
sudo exfatlabel /dev/sdc1 my_label
```

#### For ext2/3/4:
```bash
sudo e2label /dev/sdc1 my_label
```

#### For BTRFS:
at present a device label can not yet be changed without reformatting

