.. image:: https://raw.githubusercontent.com/instaloader/instaloader/master/docs/logo_heading.png

.. badges-start

|pypi| |pyversion| |license| |aur| |contributors| |downloads|

.. |pypi| image:: https://img.shields.io/pypi/v/instaloader.svg
   :alt: Instaloader PyPI Project Page
   :target: https://pypi.org/project/instaloader/

.. |license| image:: https://img.shields.io/github/license/instaloader/instaloader.svg
   :alt: MIT License
   :target: https://github.com/instaloader/instaloader/blob/master/LICENSE

.. |pyversion| image:: https://img.shields.io/pypi/pyversions/instaloader.svg
   :alt: Supported Python Versions

.. |contributors| image:: https://img.shields.io/github/contributors/instaloader/instaloader.svg
   :alt: Contributor Count
   :target: https://github.com/instaloader/instaloader/graphs/contributors

.. |aur| image:: https://img.shields.io/aur/version/instaloader.svg
   :alt: Arch User Repository Package
   :target: https://aur.archlinux.org/packages/instaloader/

.. |downloads| image:: https://pepy.tech/badge/instaloader/month
   :alt: PyPI Download Count
   :target: https://pepy.tech/project/instaloader

.. badges-end

::

    $ pip3 install instaloader

    $ instaloader profile [profile ...]

**Instaloader**

- baixa **perfis públicos e privados, hashtags, histórias de usuários, feeds e mídias salvas**,

- baixa **comentários, geotags e legendas** de cada postagem,

- detecta automaticamente **mudanças no nome do perfil** e renomeia o diretório de destino de acordo,

- permite **personalização detalhada** de filtros e onde armazenar a mídia baixada,

- retoma automaticamente iterações de download **anteriormente interrompidas**.

::

    instaloader [--comments] [--geotags]
                [--stories] [--highlights] [--tagged] [--igtv]
                [--login YOUR-USERNAME] [--fast-update]
                profile | "#hashtag" | :stories | :feed | :saved

`Instaloader Documentation <https://instaloader.github.io/>`__


Como Baixar Automaticamente Fotos do Instagram
-----------------------------------------------------


Para **baixar todas as fotos e vídeos de um perfil**, bem como a **foto do perfil**, digite no prompt do seu computador o seguinte comando:

::

    instaloader profile [profile ...]

Onde ``profile`` é o nome de um perfil que você deseja baixar. Em vez de apenas um perfil, você também pode especificar uma lista de perfis.

Para mais tarde **atualizar sua cópia local** desses perfis, você pode executar:


::

    instaloader --fast-update profile [profile ...]

Se ``--fast-update`` for fornecido, o Instaloader para ao chegar na primeira foto já baixada.

Alternativamente, você pode usar ``--latest-stamps`` para que o Instaloader armazene o tempo de cada última vez que o perfil foi baixado e apenas baixe mídia mais recente:

::

    instaloader --latest-stamps -- profile [profile ...]

Com esta opção, é possível mover ou excluir mídia baixada e ainda manter o arquivo atualizado.

Ao atualizar perfis, o Instaloader detecta automaticamente **mudanças no nome do perfil** e renomeia o diretório de destino de acordo.

O Instaloader também pode ser usado para **baixar perfis privados**. Para fazer isso, invoque-o com


::

    instaloader --login=your_username profile [profile ...]

Ao fazer login, o Instaloader **armazena os cookies da sessão** em um arquivo em seu diretório temporário, que será reutilizado mais tarde na próxima vez que ``--login`` for fornecido. Assim, você pode baixar perfis privados **não interativamente** quando já tiver um arquivo de cookie de sessão válido.


`Instaloader Documentation <https://instaloader.github.io/basic-usage.html>`__

Contributing
------------

As an open source project, Instaloader heavily depends on the contributions from
its community. See
`contributing <https://instaloader.github.io/contributing.html>`__
for how you may help Instaloader to become an even greater tool.

Supporters
----------

.. current-sponsors-start

| Instaloader is proudly sponsored by
|  `@rocketapi-io <https://github.com/rocketapi-io>`__
|  `@socialmethod <https://github.com/socialmethod>`__

See `Alex' GitHub Sponsors <https://github.com/sponsors/aandergr>`__ page for
how you can sponsor the development of Instaloader!

.. current-sponsors-end

It is a pleasure for us to share our Instaloader to the world, and we are proud
to have attracted such an active and motivating community, with so many users
who share their suggestions and ideas with us. Buying a community-sponsored beer
or coffee from time to time is very likely to further raise our passion for the
development of Instaloader.

| For Donations, we provide GitHub Sponsors page, a PayPal.Me link and a Bitcoin address.
|  GitHub Sponsors: `Sponsor @aandergr on GitHub Sponsors <https://github.com/sponsors/aandergr>`__
|  PayPal: `PayPal.me/aandergr <https://www.paypal.me/aandergr>`__
|  BTC: 1Nst4LoadeYzrKjJ1DX9CpbLXBYE9RKLwY

Disclaimer
----------

.. disclaimer-start

Instaloader is in no way affiliated with, authorized, maintained or endorsed by Instagram or any of its affiliates or
subsidiaries. This is an independent and unofficial project. Use at your own risk.

Instaloader is licensed under an MIT license. Refer to ``LICENSE`` file for more information.

.. disclaimer-end
