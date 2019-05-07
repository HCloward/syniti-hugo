+++
title = 'Copy the Assembly File to the Integrate Process Folder'
solution = 'Platform'
+++

# Copy the Assembly File to the Integrate Process Folder

A Custom template allows a user to create a mechanism for posting to any
system.

<span style="font-family: Arial, sans-serif;">A user must create all of
the associated files and code to support the Custom template.</span>

Before a Custom template can be posted, the assembly file associated
with the Custom template must be copied to a folder so that Integrate
can access it.

<span style="font-weight: bold;">NOTE</span>: To perform this task, a
user must have permission to add files to the DSP® installation on the
application server and the custom assembly must exist. Refer to [Create
a Custom Assembly](Create_a_Custom_Assembly.htm) for more information.

Copy the assembly file along with any dependent assemblies to the
Integrate Processes folder on the DSP®  Application Server. This path is
dependent on the installation, but the typical path is:

C:\\Program Files
(x86)\\BOA\\DSP\\Web\\UserArea\\E7060238-24E0-47CC-8D26-9E30AE6A2CDE\\Processes

<span style="font-weight: bold;">NOTE</span>: The GUID in the UserArea
folder is associated with Integrate. The assembly file(s) must be copied
to the folder below this GUID.

Continue with [Create a Custom
Template](Create_a_Custom_Template_Integrate.htm).
