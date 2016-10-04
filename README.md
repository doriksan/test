# [GIT TUTORIAL](https://try.github.io/levels/1/challenges/1)

### 1. Got 15 minutes and want to learn Git?

[view on github] (https://try.github.io/levels/1/challenges/1)

- it allows groups of people to work on the same documents (often code) at the same time, and without stepping on each other's toes. It's a distributed version control system.Our terminal prompt below is currently in a directory we decided to name "octobox". To initialize a Git repository here, type the following command:

`git init`

- Это позволяет группам людей работать на одних и тех же документов (часто кода) в то же время, и не наступая на пятки друг другу. Это распределенная управления версиями system.Our подсказка терминала ниже в настоящее время в каталоге мы решили назвать "octobox".

### 1.2 Checking the Status

[view on github] (https://try.github.io/levels/1/challenges/2)

- Good job! As Git just told us, our "octobox" directory now has an empty repository in /.git/. The repository is a hidden directory where Git operates.To save your progress as you go through this tutorial -- and earn a badge when you successfully complete it -- head over to create a free Code School account. We'll wait for you here.Next up, let's type the git status command to see what the current state of our project is:

`git status`

### 1.3 Adding & Committing

[view on github] (https://try.github.io/levels/1/challenges/3)

### 1.4 Adding Changes

[view on github] (https://try.github.io/levels/1/challenges/4)

- Good, it looks like our Git repository is working properly. Notice how Git says octocat.txt is "untracked"? That means Git sees that octocat.txt is a new file.To tell Git to start tracking changes made to octocat.txt, we first need to add it to the staging area by using git add.

`git add octocat.txt`

- Хорошо, это выглядит как наш репозиторий Git работает должным образом. Обратите внимание, как Git говорит octocat.txt это "несопровождаемый"? Это означает, что Git видит, что octocat.txt новый файл.Чтобы сказать Git, чтобы начать отслеживать изменения, сделанные в octocat.txt, нам сначала нужно добавить его в область размещения с помощью Git добавить.

### 1.5 Checking for Changes

[view on github] (https://try.github.io/levels/1/challenges/5)

- Good job! Git is now tracking our octocat.txt file. Let's run git status again to see where we stand:

`git status`

### 1.6 Committing

[view on github] (https://try.github.io/levels/1/challenges/6)

- Notice how Git says changes to be committed? The files listed here are in the Staging Area, and they are not in our repository yet. We could add or remove files from the stage before we store them in the repository.To store our staged changes we run the commit command with a message describing what we've changed. Let's do that now by typing:

`git commit -m "Add cute octocat story"`

- Обратите внимание, как Git говорит изменения должны быть совершены? Файлы, перечисленные здесь, находятся в промежуточной области, и они не находятся в нашем хранилище пока нет. Мы могли бы добавить или удалить файлы из стадии, прежде чем мы хранить их в хранилище.Для того, чтобы сохранить наши постановочные изменения, которые мы выполнить команду совершить с сообщением, описывающей то, что мы изменили. Давайте сделаем это сейчас.

### 1.7 Adding All Changes

[view on github] (https://try.github.io/levels/1/challenges/7)

- Great! You also can use wildcards if you want to add many files of the same type. Notice that I've added a bunch of .txt files into your directory below.I put some in a directory named "octofamily" and some others ended up in the root of our "octobox" directory. Luckily, we can add all the new files using a wildcard with git add. Don't forget the quotes!

`git add "*.txt"`

- Большой! Вы можете также использовать групповые символы, если вы хотите добавить много файлов одного и того же типа. Обратите внимание, что я добавил кучу файлов .txt в каталог ниже.Я положил некоторые в папку с именем "octofamily" и некоторые другие оказались в корне нашего каталога "octobox". К счастью, мы можем добавить все новые файлы, используя символ подстановки с ГИТ доп. Не забудьте кавычки!

### 1.8 Committing All Changes

[view on github] (https://try.github.io/levels/1/challenges/8)

`git commit -m "Add all the cotocat txt files"`

### 1.9 History

[view on github] (https://try.github.io/levels/1/challenges/9)

- So we've made a few commits. Now let's browse them to see what we changed.Fortunately for us, there's git log. Think of Git's log as a journal that remembers all the changes we've committed so far, in the order we committed them. Try running it now:

`git log`

- Таким образом, мы сделали несколько фиксаций. Теперь давайте просматривать их, чтобы увидеть, что мы изменили. К счастью для нас, есть журнал мерзавец. Подумайте о журнале Git в качестве журнала, который запоминает все изменения, которые мы совершенные до сих пор, в том порядке, мы их совершивших. Попробуйте запустить его прямо сейчас.

### 1.10 Remote Repositories

[view on github] (https://try.github.io/levels/1/challenges/10)

- Great job! We've gone ahead and created a new empty GitHub repository for you to use with Try Git at https://github.com/try-git/try_git.git. To push our local repo to the GitHub server we'll need to add a remote repository.This command takes a remote name and a repository URL, which in your case is https://github.com/try-git/try_git.git. Go ahead and run git remote add with the options below:

`git remote add origin https://github.com/try-git/try_git.git`

- Отличная работа! Мы пошли вперед и создали новый пустой репозиторий GitHub для использования с Try Git на https://github.com/try-git/try_git.git. Для того, чтобы подтолкнуть наш местный репозиторий на сервере GitHub нам нужно добавить удаленный репозиторий.Эта команда принимает имя удаленного и репозитория URL, который в вашем случае является https://github.com/try-git/try_git.git. Идите вперед и запустить Git удаленного добавить с ниже вариантов.

### 1.11 Pushing Remotely

[view on github] (https://try.github.io/levels/1/challenges/11)

- The push command tells Git where to put our commits when we're ready, and boy we're ready. So let's push our local changes to our origin repo (on GitHub). The name of our remote is origin and the default local branch name is master. The -u tells Git to remember the parameters, so that next time we can simply run git push and Git will know what to do. Go ahead and push it!

`git push -u origin master`

- Команда толчок говорит Git, где поставить наши фиксаций, когда мы готовы, и мальчик мы готовы. Так что давайте толкать наши локальные изменения нашего происхождения репо (на GitHub). Название нашего пульта дистанционного управления является происхождение и локальное имя ветви по умолчанию является ведущим. -u Говорит Git помнить параметры, так что в следующий раз мы можем просто запустить Git толчок и Git будет знать, что делать. Идите вперед и нажмите на нее!

### 1.12 Pulling Remotely

[view on github] (https://try.github.io/levels/1/challenges/12)

- Let's pretend some time has passed. We've invited other people to our GitHub project who have pulled your changes, made their own commits, and pushed them. We can check for changes on our GitHub repository and pull down any new changes by running:

`git pull origin master`

- Давайте представим, что прошло некоторое время. Мы пригласили других людей к нашему проекту GitHub, которые тянут свои изменения, сделали свои собственные фиксаций и оттеснили их. Мы можем проверить изменения на нашем хранилище GitHub и понижающий любые новые изменения, выполнив следующую команду

### 1.13 Differences

[view on github] (https://try.github.io/levels/1/challenges/13)

- Uh oh, looks like there have been some additions and changes to the octocat family. Let's take a look at what is different from our last commit by using the git diff command. In this case we want the diff of our most recent commit, which we can refer to using the HEAD pointer.

`git diff HEAD`

- Ой-ой, похоже, были некоторые дополнения и изменения в семье octocat. Давайте посмотрим на то, что отличается от нашей последней фиксации с помощью команды Git сравнения. В этом случае мы хотим, чтобы дифференциал нашего последней фиксации, который мы можем ссылаться с помощью указателя головы.

### 1.14 Staged Differences

[view on github] (https://try.github.io/levels/1/challenges/14)

- Another great use for diff is looking at changes within files that have already been staged. Remember, staged files are files we have told git that are ready to be committed. Let's use git add to stage octofamily/octodog.txt, which I just added to the family for you.

`git add octofamily/octodog.txt`

- Еще одно большое использование для показа различий смотрит на изменения в файлах, которые уже были поставлены. Помните, что поставил это файлы мы сказали ублюдка, которые готовы к фиксированию. Давайте использовать Git добавить к стадии octofamily / octodog.txt, который я только что добавленный к семье для вас.

### 1.15 Staged Differences (cont'd)

[view on github] (https://try.github.io/levels/1/challenges/15)

- Good, now go ahead and run git diff with the --staged option to see the changes you just staged. You should see that octodog.txt was created.

`git diff --staged`

- Хорошо, теперь идти вперед и запустить Git Diff с --staged опцией, чтобы увидеть изменения, которые вы просто инсценировано. Вы должны увидеть, что octodog.txt был создан.

### 1.16 Resetting the Stage

[view on github] (https://try.github.io/levels/1/challenges/16)

- So now that octodog is part of the family, octocat is all depressed. Since we love octocat more than octodog, we'll turn his frown around by removing octodog.txt. You can unstage files by using the git reset command. Go ahead and remove octofamily/octodog.txt.

`git reset octofamily/octodog.txt`

- Так что теперь octodog является частью семьи, octocat все депрессии. Так как мы любим octocat больше, чем octodog, мы повернем его нахмуриться вокруг путем удаления octodog.txt. Вы можете убрать из буфера файлов с помощью команды сброса мерзавец. Идите вперед и удалить octofamily / octodog.txt.

### 1.17 Undo

[view on github] (https://try.github.io/levels/1/challenges/17)

- git reset did a great job of unstaging octodog.txt, but you'll notice that he's still there. He's just not staged anymore. It would be great if we could go back to how things were before octodog came around and ruined the party. Files can be changed back to how they were at the last commit by using the command: git checkout -- target. Go ahead and get rid of all the changes since the last commit for octocat.txt

`git checkout -- octocat.txt`

- мерзавец сброс проделал большую работу по unstaging octodog.txt, но вы заметите, что он все еще там. Он просто не поставил больше. Было бы здорово, если бы мы могли вернуться к тому, как все было до того octodog опомнились и разрушил партию. Файлы могут быть изменены обратно, как они были на последней фиксации с помощью команды: Git Checkout - <цель>. Идите вперед и избавиться от всех изменений с момента последней фиксации для octocat.txt





