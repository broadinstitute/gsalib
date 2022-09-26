## Test environments
local OS X install, R 4.2.1
Windows Server 2022, R-devel, 64 bit (r-hub)
Ubuntu Linux 20.04.1 LTS, R-release, GCC (r-hub)
Fedora Linux, R-devel, clang, gfortran (r-hub)

## R CMD check results

There are no Errors, Warnings or Notes when testing locally.

There is 1 note which appears in all remote tests and 1 that appears only on windows.

1. The r-hub tests show one of the website links as potentially invalid, this is because our website uses
 a service which denies requests from bots.  You can verify that the link is correct if you check manually.
 We are unable to turn off bot protection or whitelist the r-hub IPs.
   
  > Found the following (possibly) invalid URLs:
  >  URL: https://gatk.broadinstitute.org/ (moved to https://gatk.broadinstitute.org/hc/en-us)
  >    From: DESCRIPTION
  >    Status: 403
  >    Message: Forbidden

2. On the windows build it shows an extraneous MikTextError file.  I'm not sure what this is or how to 
diagnose and fix it.  
 
  > checking for detritus in the temp directory ... NOTE
  > Found the following files/directories:
  >  'lastMiKTeXException'

## Downstream dependencies

There are no downstream dependencies
