# Programs - BIOS

## ACPI Sleep States (S0 - S5)

* S0: Normal Powered-On state

* S1 (Standby): The S1 sleeping state is a low wake latency sleeping state. In this state, no system context is lost (CPU or chip set) and hardware maintains all system contexts.

* S2: Not supported

* S3 (Suspend to Ram): The S3 sleeping state is a low wake latency sleeping state. This state is similar to the S1 sleeping state except that the CPU and system cache context is lost (the OS is responsible for maintaining the caches and CPU context). Control starts from the processor's reset vector after the wake event. In NCR systems, during S3, power is only provided to the USB 3.0 ports.

Note:  When the terminal resumes from an S3 state, all the USB devices re-enumerate. This causes speaker tones as if they were disconnected and then reconnected. This does not present a problem and the USB devices will continue to operate correctly.

* S4 (Suspend to Disk): The S4 state is the lowest power, longest wake latency sleeping state supported by ACPI. In order to reduce power to a minimum, it is assumed that the hardware platform has powered off all devices. Platform context is maintained.

Source

* Features > Power Management > ACPI Sleep States (S0 - S5)
  * https://onlinehelp.ncr.com/Retail/Workstations/7613/HTML/Topics/UserGuide/5.%20Power%20Management/3-ACPI%20Sleep%20States%20(S0%20-%20S5).htm
