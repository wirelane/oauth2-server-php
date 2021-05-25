oauth2-server-php
=================

[![Build Status](https://travis-ci.org/bshaffer/oauth2-server-php.svg?branch=master)](https://travis-ci.org/bshaffer/oauth2-server-php)

[![Total Downloads](https://poser.pugx.org/bshaffer/oauth2-server-php/downloads.png)](https://packagist.org/packages/bshaffer/oauth2-server-php)

View the [complete documentation](https://bshaffer.github.io/oauth2-server-php-docs/)

## FORK
The purpose of this fork is to make the \OAuth2\ResponseInterface::setStatusCode() compatible with Symfony >= 4.<br>
Currently it throws the following error when trying to use the oauth2-server-bundle from a PHP 7.4/Symfony 4/5 application:<br>
``Compile Error: Declaration of OAuth2\HttpFoundationBridge\Response::setStatusCode($statusCode, $text = NULL) must be compatible with Symfony\Component\HttpFoundation\Response::setStatusCode(int $code, $text = NULL): object``
<br>
This will raise the PHP requirement to >=7.2

