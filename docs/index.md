---
title: "How to Access the PostgreSQL Databases"
layout: "home"
description: "Since access to both the Web of Science PostgreSQL database and the Canadian Intellectual Property Office (CIPO) Patent PostgreSQL database is tied to access to supercomputers, it can only be granted after a multi-step process that ensures security and access rights"
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kara Handren
      link: https://library.utoronto.ca/staff/kara-handren
created_date: 2022-01-26
permalink: "/"  #! Remove this if not the homepage
---

# How to Access the PostgreSQL Databases

Since access to both the [Web of Science PostgreSQL database](https://mdl.library.utoronto.ca/postgresql-database-version-web-science-raw-data-xml) and the [Canadian Intellectual Property Office (CIPO) Patent PostgreSQL database](https://mdl.library.utoronto.ca/technology/text-data-mining-software/cipo-postgresql-database) is tied to access to supercomputers, it can only be granted after a multi-step process that ensures security and access rights:

1. [Get a Compute Canada account](#get-a-compute-canada-account)
2. [Opt into the Trillum service](#opt-into-the-trillum-service)
3. [Upload an SSH key to CCDB](#upload-an-ssh-key-to-ccdb)
4. [Request WoS or CIPO database access from SciNet](#request-wos-or-cipo-database-access-from-scinet)

These steps only need to be completed once to gain access, and should normally only take a few days at most to be approved.

## 1. Get a Compute Canada account 
{: #get-a-compute-canada-account}
Please visit the [Compute Canada Database (CCDB) website](https://ccdb.computecanada.ca/account_application) and apply for an account (takes a day or two to approve).  

Note: Students and postdocs need to be sponsored by their supervisor, who would need to already have a Compute Canada account (or create one first). Please [contact the Map & Data Library](https://mdl.library.utoronto.ca/about/contact-form) for assistance.

## 2. Opt in to the Trillium service
{: #opt-into-the-trillum-service}

After the Compute Canada account is approved, you should opt in to the Trillium service on the CCDB website (or use this [direct link](https://ccdb.computecanada.ca/services/opt_in)). The opt-in will be approved manually after one or two days, which will give you access to the Trillium supercomputer and other SciNet systems, as long as the SSH key has been uploaded to the CCDB website ([see next step](#upload-an-ssh-key-to-ccdb)).

## 3. Upload an SSH key to CCDB
{: #upload-an-ssh-key-to-ccdb}

Next, locate the Manage SSH Keys option on you account page on the CCDB website (or use this [direct link](https://ccdb.computecanada.ca/ssh_authorized_keys)) and upload your public SSH key. [Instructions on creating SSH key pairs](http://docs.scinet.utoronto.ca/index.php/SSH#SSH_Keys) from the SciNet Wiki can help you with this process. This wiki also contains pages with more information on [creating SSH key pairs specifically on a Windows machine](https://docs.computecanada.ca/wiki/Generating_SSH_keys_in_Windows/en), or on [Mac or Linux machines](https://docs.computecanada.ca/wiki/Using_SSH_keys_in_Linux). The Map & Data Library also provides a [quick start tutorial for creating SSH key pairs on a Mac](https://mdlutoronto.github.io/ssh-key-pairs-mac-generating/), if you need more help.

## 4. Request WoS database access from SciNet
{: #request-wos-or-cipo-database-access-from-scinet}

Finally, please send an [email to SciNet's support team](mailto:support@scinet.utoronto.ca) and let them know you would like access to the UofT-WoS database or the UofT-CIPO database. Please use your University of Toronto email address so that staff can easily identify your account. After that is approved, you will be able to connect an SQL client to these databases on the SciNet database server node (idb1)

* The Web of Science database is called 'wos'
* The Canadian Intellectual Patent Office (CIPO) database is called 'cipo'

**Please note** that if you already have access to WoS, CIPO access will be enabled by default. This does not apply in reverse - if you already have access to CIPO, you will still need to make a separate request for access to WoS. This is due to the different licenses that apply to these collections.

More [information about the database server](http://docs.scinet.utoronto.ca/index.php/Database_server) is available, as is specific information about the [UofT-WoS database structure](https://mdl.library.utoronto.ca/sites/default/public/mdldata/open/international/wos/db-structure.pdf) and the [UofT-CIPO database structure](https://maps.library.utoronto.ca/docs/postgresql/CIPO/db-structure.pdf).

If working with object-relational databases, SQL, and high performance computing environments are new to you, tutorials for both WoS and CIPO are available to help you get started:

* WoS [tutorial for Windows users](https://mdlutoronto.github.io/wos-postgresql-database-getting-started/) or [tutorial for Mac users](https://mdlutoronto.github.io/wos-postgresql-database-mac-getting-started/)
* CIPO [tutorial for Windows users](https://mdlutoronto.github.io/cipo-windows/) or [tutorial for Mac users](https://mdlutoronto.github.io/cipo-mac/)

If you have any question, feel free to [contact us](https://mdl.library.utoronto.ca/about/contact-form).

**Technique:** [Text and Data Mining](https://mdlutoronto.github.io/tutorials-search/?technique=Text+and+Data+Mining)


