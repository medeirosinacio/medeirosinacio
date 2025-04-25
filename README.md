```php

// PHP 8 is 💙, and runs on ☕️

$doug = new Person(
    name:  'Douglas Medeiros',
    email: 'eu@douglasmedeiros.dev',
    birthDate: '1993-06-05',
);

$doug->install(new Life\PackageManager([
    'curiosity',
    'coffee-dependency',
    'debugging-skills',
]));

$mySkills = new Life\Skills(
    languages:   ['PHP', 'Python', 'Bash', 'JavaScript', 'PowerShell', 'Go', 'Ruby', 'HTML/CSS', ...],
    editors:     ['PHPStorm (dark mode only)', 'VS Code', 'Notepad++ (for nostalgia)', 'Vim (how to quit?)', ...],
    frameworks:  ['HyperF', 'Bootstrap', 'Laravel', 'Yii2', 'jQuery (still alive!)', 'Flask', ...],
    databases:   ['PostgreSQL', 'MySQL', 'Redis', 'MongoDB', 'AWS Aurora', 'SQLite'],
    techStack:   [
        'Git', 'Gitlab CI/CD', 'Markdown', 'Postman',
        'Docker', 'Docker Compose', 'RabbitMQ', 'WebSocket',
        'Vagrant', 'WSL2', 'Zsh', 'Nginx', 'PHP-FPM', 'Jekyll',
        'Memcached', 'MailHog', 'CentOS', 'Ubuntu', ...
    ]
);

$developer = new Career\Developer(person: $doug, skills: $mySkills);

try {
    while ($developer->hasEnergy() || $developer->hasCoffee()) {
        $developer->code();
    }
} catch (Life\Exceptions\BurnoutException $e) {
    $developer->rest();
    $developer->hydrate();
    $developer->comeBackStronger();
}

```
