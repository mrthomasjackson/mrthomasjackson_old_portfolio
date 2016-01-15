# MrThomasJackson » Portfolio

#### Server Requirements:
-----
  1. Ubuntu 14.04
  2. Git
  3. PHP 5.6 (for future development)
  4. Apache
  5. MySQL (for future development)
  6. Composer
  7. Node (With PM2, Bower, Grunt, and Gulp)


#### Branches:
-----
  * Master - Used for production environment.
  * Dev - Used for development environment.

#### Deployment Plan:
-----
  1. Merge Dev Branch into Master
   * $ git checkout master - Switches to the local master branch
   * $ git pull dev master - Resolve any conflicts
    * $ git add -A
    * $ git commit -am ‘Relevant detailed commit message.’
    * $ git pull github master
   * $ git merge newFeatureName
  2. Test - Determine if merge was successful
   $ git push dev master - Only when setermined a stable release
  3. Tag
    * $ git tag -a vX.X.X -m ‘Release Code or Feature Name ’
    * $ git push github --tags
