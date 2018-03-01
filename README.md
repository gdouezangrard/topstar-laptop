# Topstar Laptop ACPI Extras

Provide WLAN LED workaround for Topstar U931/RVP7 laptops.

## Build

```console
$ make
```

## Usage

Before loading the module, you might need to unload the kernel built-in driver
with:

```console
$ rmmod topstar_laptop
```

Then load the new kernel driver:

```console
$ modprobe sparse-keymap
$ insmod topstar-laptop.ko
```
