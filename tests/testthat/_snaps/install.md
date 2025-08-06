# renv warns when installing an already-loaded package

    Code
      install("bread@0.1.0")
    Output
      The following package(s) will be installed:
      - bread [0.1.0]
      These packages will be installed into "<tempdir>/<renv-library>".
      
      # Installing packages ---
      - Installing bread 0.1.0 ...                    OK [copied from cache in XXs]
      Successfully installed 1 package in XXXX seconds.
      
      The following loaded package(s) have been updated:
      - bread
      Restart your R session to use the new versions.
      

# install has user-friendly output

    Code
      install()
    Output
      # Downloading packages ---
      - Downloading breakfast 1.0.0 from CRAN ...     OK [XXXX bytes in XXs]
      - Downloading oatmeal 1.0.0 from CRAN ...       OK [XXXX bytes in XXs]
      - Downloading toast 1.0.0 from CRAN ...         OK [XXXX bytes in XXs]
      - Downloading bread 1.0.0 from CRAN ...         OK [XXXX bytes in XXs]
      Successfully downloaded 4 packages in XXXX seconds.
      
      The following package(s) will be installed:
      - bread     [1.0.0]
      - breakfast [1.0.0]
      - oatmeal   [1.0.0]
      - toast     [1.0.0]
      These packages will be installed into "<tempdir>/<renv-library>".
      
      # Installing packages ---
      - Installing oatmeal 1.0.0 ...                  OK [built from source and cached in XXs]
      - Installing bread 1.0.0 ...                    OK [built from source and cached in XXs]
      - Installing toast 1.0.0 ...                    OK [built from source and cached in XXs]
      - Installing breakfast 1.0.0 ...                OK [built from source and cached in XXs]
      Successfully installed 4 packages in XXXX seconds.

---

    Code
      install()
    Output
      The following package(s) will be installed:
      - bread     [1.0.0]
      - breakfast [1.0.0]
      - oatmeal   [1.0.0]
      - toast     [1.0.0]
      These packages will be installed into "<tempdir>/<renv-library>".
      
      # Installing packages ---
      - Installing oatmeal 1.0.0 ...                  OK [copied from cache in XXs]
      - Installing bread 1.0.0 ...                    OK [copied from cache in XXs]
      - Installing toast 1.0.0 ...                    OK [copied from cache in XXs]
      - Installing breakfast 1.0.0 ...                OK [copied from cache in XXs]
      Successfully installed 4 packages in XXXX seconds.

