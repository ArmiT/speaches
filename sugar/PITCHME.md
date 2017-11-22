# Sugar

---

## Introduction

+++

### What is it?

Safe storage for important data

+++

### What it can?

* encrypt and decrypt messages and credentials
* user Authentication with OAuth
* manage clients, projects, sites, messages and credentials
* enhanced search
* secure communication between clients and company

---

## Some abstracts

+++

### Code metrics

| main | front | public
|------|-------|-------
code | lines 15684 | 12862  | 2226
complexity | 1.03  | 1.15   | 1.04
copy-paste | 3.62% | 3.65%  | 3.01%
coverage |   87.1% | 89.21% | 88.5%

+++

### security metrics

* tls everywhere
* hard csp settings
* cors
* X-headers
* securing data with encryption
* hacks - spellcheck, Hyperscript, direct loading, rel="nooppener noreferer"

+++

### mozilla observatory

+++?image=sugar/img/mobservatory-sugar.png&size=auto

+++?image=sugar/img/mobservatory-sber.png&size=auto

+++?image=sugar/img/mobservatory-wc.png&size=auto

+++

### Data metrics / main

* 8 entities total 
* 61 users
* 1117 clients
* 2965 projects
* 3066 messages

---

## Architecture

+++?image=sugar/img/structure.png&size=auto

+++?image=sugar/img/security-concept.png&size=auto

+++

### Algorithms

* keys pairs - RSA 4096
* symmetric encryption - AES256 (CBC & GSM)

+++

### Data model

* users
* clients
 * projects
  * messages
  * sites
   * domains
* credentials
* encryptedPayload

---

## Tech stack

* javascript (node-boilerplate, spa-boilerplate)
* html (Hyperscript), pure css
* rethinkdb, redis
* nginx
* docker

+++?image=sugar/img/clean-architecture.png&size=auto

+++?image=sugar/img/clean-architecture2.jpg&size=auto

+++?image=sugar/img/app-architecture.png&size=auto

+++?image=sugar/img/files-structure.png&size=auto

+++

## Flow

+++?image=sugar/img/flow.png&size=auto 

---?include=repo-link.md
