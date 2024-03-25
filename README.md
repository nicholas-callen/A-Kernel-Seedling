# A Kernel Seedling
Nicholas Callen, UID 405739681

## Building
```shell
make
```
 (has to be done in the directory for lab0)

## Running
```shell
sudo insmod proc_count.ko
cat /proc/count
```
Printed back a single number, for me it was 135.

## Cleaning Up
```shell
sudo rmmod proc_count 
```
(removes the inserted module from the kernel)

## Testing
```python
python -m unittest
```
Ran 3 tests in about 20 seconds, result was OK.
Repeated this 10 times to verify result, on average took roughly 20 seconds as well.

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
Linux 5.14.8-arch1-1 #1 SMP PREEMPT