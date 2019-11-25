# Basic concepts

There are few basic concepts that are important to understand the **UpdateHub** engine. Those basic concepts are detailed below:

### Device

The `Device` represents your physical device. It has multiple characteristics which are tracked on the management platform, as such: hardware type, unique identifier, runtime attributes and more.

### Organization

An `Organization` means that you have a entity to manager your products. It's not a company for business purposes.

### Package

A software version, including the filesystem image, bootloader or any other objects, is represented by a `Package`.

### Rollout

The `Rollout` is essentially a deployment plan. It can be simple as "send version 2.0 for all devices" or complex selecting specific filters and enforcing a gradual deployment across the devices set.

### Product

The basis that connects all together through the **UpdateHub** is the`Product`. Essentially the Product includes one or multiple `Devices` and for each of them there is a `Package` version that may be updated using a `Rollout`.
