# Owl Forest

[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

![image](https://github.com/user-attachments/assets/4192e61d-a96c-4490-8d39-04ffac7ad412)

Premissa do jogo ; Certo dia, duas corujas irmãs fogem de seu ninho para explorar a floresta encantada de Mega city, depois de sobrevoarem a cidade por muito tempo, eles finalmente chegam à floresta. Lá a irmã mais nova Anne percebe que está sozinha e que não consegue enxergar mais seu irmão por perto. Depois de muito chiar para encontrá-lo, Anne percebe que seu irmão Brian havia deixado algo para trás para marcar seu caminho para voltar. Brian deixou seu rastro com vários corações comestíveis pelos lugares, para que eles o guiassem até seu ninho novamente. Durante a procura de Anne, seu irmão já está voltando para encontrá-la e destruindo o caminho que tinha feito, comendo os corações. Durante esses desencontros, os irmãos vão coletando todos os corações até finalmente se encontrarem e voltarem para casa juntos e em segurança. 


## Configuração do ambiente

Proxy reverso NGINX:

```
location / {
	proxy_pass http://localhost:3000/;
	proxy_http_version 1.1;
	proxy_set_header Upgrade $http_upgrade;
	proxy_set_header Connection "Upgrade";
	proxy_set_header Host $host;
}
```

Servidor do jogo via `systemd`:

```ini
[Unit]
Description=<Descritivo>
Documentation=<URL do repositório>
After=network.target

[Service]
Environment=PORT=3000
Type=simple
WorkingDirectory=<diretório local do repositório>
ExecStart=<caminho do npm> start
Restart=on-failure

[Install]
WantedBy=multi-user.target
```

## Equipes

| Equipe | Jogo |
|-|-|
| [Bernardo, Filipe e Vitor Ademir](https://github.com/VFB-Corporation) | [Jogo](https://github.com/VFB-Corporation/JOGO) |
| [Mariana e Vitor Hugo](https://github.com/mvplay-s) | [Pilatus](https://github.com/mvplay-s/Pilatus) |
| [Náthally e Guilherme](https://github.com/vimdoalegrete) | [jogo](https://github.com/vimdoalegrete/jogo) | 
| [Davi e Gabriel](https://github.com/huntersofancientbeasts)|[Hunters of Ancient Beasts](https://github.com/huntersofancientbeasts/jogo) |
| [Erika e Yago](https://github.com/erikayago) | [jogo](https://github.com/erikayago/jogo) |
| [Gustavo e Vitória]() | [jogo](https://github.com/tangram-game/jogo) |
| [Leandro e Nikolas](https://github.com/nlentertainment) | [jogo](https://github.com/nlentertainment/jogo) |
