# X99 HACKINTOSH EFI CATALINA AND BIG SUR
X99 Opencore config repository for Catalina and Big Sur



If you wanna give a smile to me:

<a href="https://buymeacoffee.com/UHSEGfn" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>





Opencore Version: 0.6.4

Compatible With:

# Catalina
 - 10.15.6
 - 10.15.7

# Big Sur
 - 11.0.1

# Included Full Patched DSDT for

 - HUANANZHI X99-F8 AND HUANANZHI X99-TF "DSDT-HUANANZHI.aml"

# Included SSDT for:

 - Disabling PCI Uncore Bridges  "SSDT-UNC0.aml" (Causes KernelPanic ^19.7.0 Kernels)
 - Renaming CPU to CP0 PCI Uncore Bridges  "X99-CP00-XCPM.aml" (As a Real MAC)

# HASWELL/BROADWELL (E/EP) Power Management

 - On KERNEL>Cpuid1Mask
  Replace:

   F2060300 00000000 00000000 00000000 for HASWELL-E/EP
   
   F1060400 00000000 00000000 00000000 for BROADWELL-E/EP

 - On KERNEL>Patch

	HASWELL-E/EP
   	 xcpm_bootstrap_HASwell-E (c) Pike R.  		(ENABLE)
     xcpm_bootstrap_Broadwell-E (c) Pike R.  	(DISABLE)

    BROADWELL-E/EP
   	 xcpm_bootstrap_HASwell-E (c) Pike R.  		(DISABLE)
     xcpm_bootstrap_Broadwell-E (c) Pike R.  	(ENABLE)

     Remember that there is 2 of each patch one for CATALINA and the other for BIG SUR

# Credits
  
  - Mald0n for introducing me to hackintosh and giving me my first pre-made folder (Olarila.com)
  - Nmano for mantaining actively Kernel Patches for x99/x299 between Mac OS versions
  - Pike R for introducing Patches for x79/x99/x299 
  - Acidanthera team for developing Opencore and most Kexts
  - Apple for developing MacOS


