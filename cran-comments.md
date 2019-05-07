## Test environments
* local OS X install, R 3.6.0
* ubuntu 14.04 (on travis-ci), R 3.6.0
* win-builder (devel and release)

## R CMD check results

0 errors | 0 warnings | 1 note

* This is a new release.

## On win-builder:

I got:

```
Error: .onLoad failed in loadNamespace() for 'pillar', details:
  call: NULL
  error: .onLoad failed in loadNamespace() for 'vctrs', details:
  call: get(genname, envir = envir)
  error: object 'type_sum' not found
Execution halted
ERROR: lazy loading failed for package 'glancedata'
* removing 'd:/RCompile/CRANguest/R-devel/lib/glancedata'
```

I did not get that error in any other test environment.

## On r_hub

I got this note:

```
N  checking CRAN incoming feasibility
   Maintainer: 'Guillermo Basulto-Elias <guillermobasulto@gmail.com>'
   New submission
```
