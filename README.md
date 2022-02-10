# Contributors' trombinoscope

## About

This is a bash script which uses `jq` and `sed` to replace contributors list in 
a file. It's meant to be used in GitHub actions.

## Usage

Place these HTML comments to delimit the contributors list:
> \<\!-- start_contributors -->  
> \<\!-- end_contributors -->

The script will insert the contributors list between these markers. 

## Test

An easy way to test the result is to use [pandoc]:  
`pandoc -s -f gfm -t html5 -o output.html README.md`

## Contributors
<!-- start_contributors key:value mode:link -->
  * [@SaphireVert](https://github.com/SaphireVert)
  * [@D4rkHeart](https://github.com/D4rkHeart)
  * [@Azecko](https://github.com/Azecko)
  * [@multiscan](https://github.com/multiscan)
  * [@JaavLex](https://github.com/JaavLex)
  * [@ponsfrilus](https://github.com/ponsfrilus)
  * [@crazylady2004](https://github.com/crazylady2004)
<!-- end_contributors -->

## Something else


[github actions]: https://pandoc.org/MANUAL.html
[pandoc]: https://pandoc.org/MANUAL.html
