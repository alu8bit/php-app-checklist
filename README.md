# PHP application checklist

List of useful approaches to improve and check your PHP-based project.

## Table of Contents
- [Base section](#base-section)
- [Architecture section](#architecture-section)
- [Code section](#code-section)
- [Database section](#database-section)
- [Frontend section](#frontend-section)
- [Security section](#security-section)
- [Administration section](#administration-section)
- [Team section](#team-section)
- [Tools section](#tools-section)
- [Metrics section](#metrics-section)
- [Scalable and performance section](#scalable-and-performance-section)

### Base section
* Do you use the latest stable PHP version?
  * [Supported versions](http://php.net/supported-versions.php)
* Try to be aware of last changes, technologies and tools.
  * [PHP: The Right Way](http://www.phptherightway.com/) - best PHP practices.
  * [Awesome PHP](https://github.com/ziadoz/awesome-php) - list of PHP libraries, resources and shiny things.
  * [The twelve-factor app](https://www.12factor.net/) - Methodology for building software-as-a-service apps.

### Architecture section
* Do you use well supported, not outdated and popular PHP framework, not your own?
  * [Laravel](https://laravel.com), [Symfony](https://symfony.com), [Zend Framework](https://framework.zend.com/), [Yii](https://www.yiiframework.com) and etc. - frameworks.
  * [Slim](https://www.slimframework.com), [Lumen](https://www.slimframework.com) and etc. - microframeworks.
* Do you have a lot of custom solutions? Maybe it’s easier to use external libraries, PHP extensions and SPL?
  * [The PHP package repository](https://packagist.org)
  * [PHP extentions](http://php.net/manual/en/extensions.php)
  * [Standard PHP Library](http://php.net/manual/en/book.spl.php)
* Do you use dependency manager?
  * [Composer](https://getcomposer.org), [One page Doc](http://composer.json.jolicode.com), [17 useful Composer tips](https://blog.martinhujer.cz/17-tips-for-using-composer-efficiently/)
* Try to follow by best coding practices like SOLID, KISS, DRY and etc.
* Try to create common solution, not unique.
  * [PHP Package Checklist](http://phppackagechecklist.com/#1,2,3,4,5,6,7,8,9,10,11,12,13,14)

### Code section
* Do you use code version control system and appropriate branching model?
  * [Git](https://git-scm.com), [Mercurial](https://www.mercurial-scm.org) - source control management tools.
  * [Git Flow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow), [GitHub Flow](http://scottchacon.com/2011/08/31/github-flow.html), [GitLab Flow](https://about.gitlab.com/2014/09/29/gitlab-flow/) - branching models.
* Do you have common code style? Does it apply automatically?
  * [PHP CS Fixer](http://cs.sensiolabs.org), [PHP Code Sniffer](https://github.com/squizlabs/PHP_CodeSniffer)
* Do you have automatically generated code documentation for your app and API?
* Do you have code review and acceptance policy?
* Do you have code auto-completion and live templates, skeletons for commonly used files?

### Database section
* Do you use ORM model to not depend on database type? 
* Do you have any backup system? 
* Do have clear migration system? 

### Frontend section
* Do you use any template engine? 
* Do you use any up to date frontend framework? 
* Do you use last HTML version? 

### Security section
* Try to follow [OWASP Top 10](https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project).
* Always use protected connection for your web application.
  * [Let’s Encrypt](https://letsencrypt.org), [SSL For Free](https://www.sslforfree.com) - free SSL certificates.
* Do you check project code for vulnerabilities?
  * [RIPS](http://rips-scanner.sourceforge.net), [composer.lock checker](https://security.sensiolabs.org/check)
* Do you have password and other sensitive data saving policy?
  * [OWASP Cheat Sheet](https://www.owasp.org/index.php/Password_Storage_Cheat_Sheet), [Hashing](http://php.net/manual/en/faq.passwords.php)

### Administration section
* Do you dev or testing environment and splited configuration for them? 
* Try to use containerisation. 
* Do you have any hardware monitoring system? 
* Do you have logging system? 
* Do you have log prioritization? 
* Do you have any notification system when errors occurs? 

### Team section
* Do you have clear team structure? 
* Do you have problems in communication?
* Do you use bug reporting system? 
* Do you use predefined templates for bug report description? 

### Tools section
* Do you have connected debugging tool for your application? 
* Do you use deployment tool? 
* Maybe it will be useful to integrate CI in your development process. 

### Metrics section
* Do you know your code coverage for tests?
* Do you know your code quality? Try to use static code analysis tools.
* Do you know your team productivity and development score?

### Scalable and performance section
* Try to use queue system for better performance. 
* Try to use cache system.
* Try to use async php.
