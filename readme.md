# Step 1 is always dism.
Dism /online /Cleanup-Image /StartComponentCleanup

Dism /Online /Cleanup-Image /ScanHealth

Dism /Online /Cleanup-Image /RestoreHealth

# then the great gods of fixing!

sfc /scannow

chkdsk /F
