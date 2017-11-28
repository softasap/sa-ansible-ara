sa-ansible-ara
==============

[![Build Status](https://travis-ci.org/softasap/sa-ansible-ara.svg?branch=master)](https://travis-ci.org/softasap/sa-ansible-ara)


Basic role for openstack ara install


Example of usage:

Simple

```YAML

     - {
         role: "sa-ansible-ara"
       }


```

Advanced

```YAML

     - {
         role: "sa-ansible-ara",
         option_configure_startup: true,
         option_configure_nginx: true,

         ara_user: ara,
         ara_home: "/home/{{ara_user}}",
         ara_virtual_env: "/home/{{ara_user}}/virtual_envs",
         ara_log_dir: /var/log/ara,

         ara_ssl_key: ara,
         ara_ssl_crt: ara,
         ara_domain: ara.voronenko.info
       }


```



Usage with ansible galaxy workflow
----------------------------------

If you installed the `sa-ansible-ara` role using the command


`
   ansible-galaxy install softasap.sa-ansible-ara
`

the role will be available in the folder `library/softasap.sa-ansible-ara`
Please adjust the path accordingly.

```YAML

     - {
         role: "softasap.sa-ansible-ara"
       }

```




Copyright and license
---------------------

Code is dual licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) and the [MIT License] (http://opensource.org/licenses/MIT). Choose the one that suits you best.

Reach us:

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)

Join gitter discussion channel at [Gitter](https://gitter.im/softasap)

Discover other roles at  http://www.softasap.com/roles/registry_generated.html

visit our blog at http://www.softasap.com/blog/archive.html
