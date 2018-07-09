# Exit Codes

| Exit Codes | Reason |
|:----------:|:-------|
| 1- 10 | Script cannot run on the system |
|  1 | Dependencies are not met |
|  2 | Script not running as root |
|  8 | remote get operation failed. |
| 10-19 | Not Running with right configuration or internal flags |
| 11 | Unsupported Architecture |
| 12 | End of Life release |
| 14 | No Internet connection |
| 15 | Conflicting apps are running |
| 16 | Distribution is  Not supported |
| 17 | Distribution is not yet supported. But will be in the future. |
| 19 | Internal Functions: Invalid arguments |
| 20- 254 | User configuration / Run-time errors |
| 20 | Purge function is  called without -d flag |
| 21 | Failed to install dependencies |
| 22 | Invalid flag passed |
| 23 | Invalid argument position. |
| 24 | Not Running the latest version |
| 28 | Getting API response failed |
| 29 | Stat reporting failed |
| 35 | Not a valid config file type |
| 36 | file defined does not exist/not accessible |
| 37 | Configuration error. Expects Boolean but found something else. |
| 38 | Failed to delete a file |
| 255 | Test Exit code |
