# X99 HACKINTOSH EFI CATALINA AND BIG SUR
X99 Opencore config repository for Catalina and Big Sur



If you wanna give a smile to me:

<a href="https://www.paypal.com/donate?business=7KKQS9KBSAMNE&item_name=Maintaining+HEDT+hackintosh+related+repositories&currency_code=USD" target="_blank">
  <img width="50" height="auto" src="https://raw.githubusercontent.com/stefan-niedermann/paypal-donate-button/master/paypal-donate-button.png" alt="Donate with PayPal"/>
</a>





Opencore Version: 0.6.4

Compatible With:

# Catalina
 - 10.15.6
 - 10.15.7

# Big Sur
 - 11.0.1

# Included Full Patched DSDT/SSDT Depending on your Motherboard:

 - HUANANZHI FOLDER F8 or TF "DSDT-HUANANZHI.aml"
 - MACHINIST FOLDER, Bunch of SSDT
 - JINGSHA SZMZ X99 Dual, Bunch of SSDT

 All of them tested with BIOS-IEGINEER's BIOSES

 <a href="https://github.com/BIOS-iEngineer" target="_blank">https://github.com/BIOS-iEngineer</a>

 ```
Copy all them from the specific ACPI/"FOLDER" depending on your motherboard to ACPI/ and activate them on config.plist>ACPI>add 
 ```

# Included SSDT for:

 - Disabling PCI Uncore Bridges  "SSDT-UNC0.aml" (Causes KernelPanic ^19.7.0 Kernels) (Universal)
 - Renaming CPU to CP00 PCI Uncore Bridges  "X99-CP00-XCPM.aml" (As a Real MAC) (Universal)


 ```
Universal SSDT can be used on any x99 motherboard (Common issues)
 ```

# HASWELL/BROADWELL (E/EP) Power Management

 - On KERNEL>Cpuid1Mask
  Replace:

   F2060300 00000000 00000000 00000000 for HASWELL-E/EP
   
   F1060400 00000000 00000000 00000000 for BROADWELL-E/EP

   57060500 00000000 00000000 00000000 for CASCADE LAKE-X
   
   54060500 00000000 00000000 00000000 for SKYLAKE-X/H

   E4060300 00000000 00000000 00000000 for IVY BRIDGE-E/EN/EP

 - On KERNEL>Patch

	FIND YOUR XCPM_BOOTSTRAP_PATCH ENABLE IT AND DISABLE THE REST OF XCPM_BOOTSTRAP Patches for the other processors
  

```
 Remember that there is 2 of each patch one for CATALINA and the other for BIG SUR
```
# Credits
  
  - Mald0n for introducing me to hackintosh and giving me my first pre-made folder (Olarila.com)
  - Nmano for mantaining actively Kernel Patches for x99/x299 between Mac OS versions (insanelymac.com)
  - e97 for it's original HackPro X99 System post which was of the first X99 Successful build which inspired us (insanelymac.com)
  - RemB for it's UNC0-SSDT.aml in order to disable Uncore PCI Bridges (insanelymac.com)
  - Pike R for introducing Patches for x79/x99/x299 
  - Acidanthera team for developing Opencore and most Kexts (github.com/acidanthera)
  - Apple for developing MacOS


