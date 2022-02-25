# Netboot.xyz configs
[Netboot.xyz](https://netboot.xyz/)
is a platform for booting multiple operating systems and utilites over the network with
[PXE](https://en.wikipedia.org/wiki/Preboot_Execution_Environment).

The [custom.ipxe](./custom.ipxe) provides my custom boot options for Netboot.xyz.
(However, it's just a Hello World for now.)

There are two ways to get the configs to work on your device.
The first is to compile the iPXE image yourself and set the `github_user` variable for the build.
The other way is to start the image and go to *Tools -> Utilities -> netboot.xyz tools* and set the username there.
The way Netboot.xyz finds these files is by looking for the URL:
```
https://raw.githubusercontent.com/${github_user}/netboot.xyz-custom/master/custom.ipxe
```

Please see the [template repository](https://github.com/netbootxyz/netboot.xyz-custom) for examples on how to create custom ipxe files.
