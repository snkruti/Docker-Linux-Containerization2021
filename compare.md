# Containerization or virtualization

<img src="https://lwstatic-a.akamaihd.net/kb/wp-content/uploads/2019/12/vm-vs-containers.png" width="500" height="350" />

## Virtualization

* More secure and fully isolated

* **Virtualization** allows you to run multiple operating systems on one physical server's hardware

* **Virtual machines** are perfect for supporting applications that need the full functionality of an operating system when you choose to run several applications on a server or have a wide range of operating systems to accommodate them.

*  **Virtual machine** have a longer lifecycle and are better used for longer periods of time than containers.

## Containerization

* Less secure and isolated at the process level

* **containerization** allows you to install multiple applications on a single virtual machine or server using the same operating system.

* **Containers** are a better choice if the main goal is to minimize the number of servers you are using for differnt applications.

* For activities with a much shorter lifecycle, **containers** are an excellent option.
They are perfect for tasks that can only take a few hours, with their quick set-up time.

## Conclusion

Containerization and virtualization vary in several aspects, but the key difference is that containers in a single OS instance provide a way to virtualize an OS to run multiple workloads. With VMs, to run several OS instances, the hardware is virtualized. The container's speed, agility, and portability make it another instrument for streamlining the production of software.
