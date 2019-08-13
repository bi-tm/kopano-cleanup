kopano-cleanup
==============

The following scripts allow you to automatically delete or archive all items older than x days in a users **Junk E-mail** and **Deleted Items** folder.

Parameters
```python
  -f NAME, --folder=NAME             Specify folder
  --user=USER                        Run script for user
  --wastebasket                      Run cleanup script for the wastebasket
                                     folder
  --archive=ARCHIVE                  instead of removing items archive them
                                     into this folder
  --junk                             Run cleanup script for the junk folder
  --sent                             Run cleanup script for the sent folder
  --force                            Force items without date to be removed
  --days=DAYS                        Delete older then x days
  --verbose                          Verbose mode
  --dry-run                          Run script in dry mode
  --progressbar                      Show progressbar
  --recursive                        Delete items in subfolder,
                                     delete subfolder itself, if it is empty.

```

## Usage
delete
```python
python cleanup.py --user username --junk --wastebasket --days days   
```

archive
```python
python cleanup.py --user username --junk --wastebasket --days days  --archive foldername

```

