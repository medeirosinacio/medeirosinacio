```php

$eu = new Pessoa(
    nome:  'Douglas Medeiros',
    email: 'medeirosinacio@outlook.com',
    idade:   27,
);

$eu->setarStatus(new Vida\Status(
    estudando:   ['Laravel 8', 'Clean Code'],
    interessado: ['vue.js', 'Flask'],
    objetivo:    ['Contribuir para a comunicade', 'Larafull']
));

$habilidades = new Vida\Habilidades(
    linguagens:  ['PHP', 'Python', 'Bash', 'HTML/CSS', 'Javascript', 'Powershell'],
    editores:    ['PHPStorm', 'VsCode', 'Notepad++', 'Vim'],
    frameworks:  ['Bootstrap', 'Laravel', 'Yii2', 'Jquery'],
    banco:       ['PostgreSQL', 'MySql'],
    tecnologia:  [
                    'Git', 'Gitlab CI/CD', 'Markdown', 'Postman',
                    'Docker', 'Docker Compose', 'RabbitMQ', 'Redis',
                    'Vagrant', 'WSL2', 'Zsh', 'Nginx', 'PHP-FPM',
                    'Memcached', 'Maillhog', 'CentOS', 'Ubuntu'
                 ]
);

$dev = new Profissao\Desenvolvedor($eu, $habilidades);

while($dev->temCafé())  
{
  $dev->codar();
}

```
