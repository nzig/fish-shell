.. _cmd-prompt_login:

prompt_login - describe the login suitable for prompt
=====================================================

Synopsis
--------

``prompt_login``

Description
-----------

``prompt_login`` is a function to describe the current login. It will show the user, the host and also whether the shell is running in a chroot (currently debian's debian_chroot is supported).

Examples
--------
::

    function fish_prompt
        echo -n (prompt_login) (prompt_pwd) '$ '
    end

::

    >_ prompt_login
    root@bananablaster
