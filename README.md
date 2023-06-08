# Mastodon Bot: Rastreador do Twitter

## Introdução

Mastodon Bot rastreando tweets de contas do Twitter.

Isso foi desenvolvido inicialmente para coletar avisos oficiais de um jogo online. Infelizmente, não havia outros canais alternativos para rastrear informações.

## Isenção de responsabilidade

**Evite criar bots para rastrear indivíduos.**

Não me responsabilizo por quaisquer danos ou perdas decorrentes do uso do meu projeto.

É altamente recomendável definir a visibilidade do toot como `private` para garantir que seu bot não esteja poluindo toda a Federação.


## Instalação e uso

O projeto é testado em Python 3.10, Debian 11

```bash
$ # Instalar dependências
$ pip3 install -r requisitos.txt
$ # Configure seu arquivo de ambiente (consulte .env.example)
$ cp .env.example .env
$vi.env
$ # Execute e veja se tudo funciona.
$ python3 main.py
```

Você também pode manter `systemd/mastodonbot.service` para executar o bot como daemon.

```bash
$ cp systemd/mastodonbot.service /etc/systemd/system/mastodonbot.service
$ systemctl daemon-reload
$ systemctl habilita mastodonbot
$ systemctl start mastodonbot
```
# FindTweet
