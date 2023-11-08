```php

// PHP 8 is <3

$developer = new Dev(
    name:  'Douglas Medeiros',
    email: 'eu@douglasmedeiros.dev',
    age:   30
);

$developer->setStatus(new Life\Status(
    learning:   ['Java', 'Software Architecture'],
    exploring:  ['vue.js', 'Flask'],
    aiming:     ['Empower the Community']
));

$mySkills = new Life\Skills(
    languages:   ['PHP', 'Python', 'Bash', 'HTML/CSS', 'JavaScript', 'PowerShell'],
    editors:     ['PHPStorm', 'VS Code', 'Notepad++', 'Vim'],
    frameworks:  ['Bootstrap', 'Laravel', 'Yii2', 'jQuery'],
    databases:   ['PostgreSQL', 'MySQL', 'Redis'],
    techStack:   [
        'Git', 'Gitlab CI/CD', 'Markdown', 'Postman',
        'Docker', 'Docker Compose', 'RabbitMQ', 'WebSocket',
        'Vagrant', 'WSL2', 'Zsh', 'Nginx', 'PHP-FPM', 'Jekyll',
        'Memcached', 'MailHog', 'CentOS', 'Ubuntu'
    ]
);

$developerRole = new Career\Developer(person: $developer, skills: $mySkills);

while ($developerRole->hasCoffee())  
{
    $developerRole->code();
}

```
