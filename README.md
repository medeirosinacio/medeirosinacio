```php

// PHP 8 is <3

$eu = new Pessoa(
    nome:  'Douglas Medeiros',
    email: 'medeirosinacio@outlook.com',
    idade:  29,
);

$eu->setarStatus(new Vida\Status(
    estudando:   ['Laravel 9', 'Clean Code'],
    interessado: ['vue.js', 'Flask'],
    objetivo:    ['Contribuir para a comunidade', 'LaraAD']
));

$minhasHabilidades = new Vida\Habilidades(
    linguagens:  ['PHP', 'Python', 'Bash', 'HTML/CSS', 'Javascript', 'Powershell'],
    editores:    ['PHPStorm', 'VsCode', 'Notepad++', 'Vim'],
    frameworks:  ['Bootstrap', 'Laravel', 'Yii2', 'Jquery'],
    banco:       ['PostgreSQL', 'MySql', 'Redis'],
    tecnologia:  [
                    'Git', 'Gitlab CI/CD', 'Markdown', 'Postman',
                    'Docker', 'Docker Compose', 'RabbitMQ', 'Websocket',
                    'Vagrant', 'WSL2', 'Zsh', 'Nginx', 'PHP-FPM', 'Jekyll'
                    'Memcached', 'Maillhog', 'CentOS', 'Ubuntu'
                 ]
);

$dev = new Profissao\Desenvolvedor(pessoa: $eu, habilidades: $minhasHabilidades);

while($dev->temCafé())  
{
  $dev->codar();
}

```
