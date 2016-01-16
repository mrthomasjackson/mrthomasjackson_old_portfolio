# MrThomasJackson's Portfolio

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
  1. Merge dev into master
   * $ git checkout master
   * $ git merge dev master
   * $ git push
  2. Push Master to Staging Server
   * $ git push staging
   * Test in stage enviornment.
   * $ git tag -a vX.X.X -m ‘Release Code or Feature Name ’
  3. Push Master to Production Server
   * $ git push production
   * $ git push github --tags
   * Test in production enviornment.
