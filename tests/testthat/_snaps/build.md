# warnings can be turned into errors

    Code
      build(file.path(src, "testDummy"), dest_path = dest, quiet = TRUE)
    Message <cliMessage>
      ! Stopping as requested for a warning during `R CMD build`.
      ! The full output is printed below.
      * checking for file '<file>' ... OK
      * preparing 'testDummy':
      * checking DESCRIPTION meta-information ... OK
      * checking for LF line-endings in source and make files and shell scripts
      * checking for empty or unneeded directories
        NB: this package now depends on R (>= 3.5.0)
        WARNING: Added dependency on R >= 3.5.0 because serialized objects in
        serialize/load version 3 cannot be read in older versions of R.
        File(s) containing such objects:
          'testDummy/inst/testthat-problems.rds'
      * building 'testDummy_0.1.tar.gz'
      
    Error <simpleError>
      converted from `R CMD build` warning.

