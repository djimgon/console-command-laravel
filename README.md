# console-command-laravel

# Создаем консольную команду
php artisan make:command User/VerifyCommand


class VerifyCommand extends Command
{
    protected $signature = 'user:verify {email}';

    protected $description = 'Команда, которая верифицирует пользователя';

    public function handle() : bool
    {
        $this->info('success!');

        return true;
    }
}

{email} это дополнительное значение для команды
