<div class="span16">
          <h2>What are Git hooks?</h2>
          <p>
            Git hooks are scripts that Git executes before or after events such
            as: <b>commit</b>, <b>push</b>, and <b>receive</b>. Git hooks are a
            built-in feature - no need to download anything. Git hooks are run
            locally.
          </p>

          <p>
            These hook scripts are only limited by a developer's imagination.
            Some example hook scripts include:
          </p>

          <ul>
            <li>
              <b>pre-commit</b>: Check the commit message for spelling errors.
            </li>
            <li><b>pre-receive</b>: Enforce project coding standards.</li>
            <li><b>post-commit</b>: Email/SMS team members of a new commit.</li>
            <li><b>post-receive</b>: Push the code to production.</li>
          </ul>

          <hr class="soften">
          <h2>How do git hooks work?</h2>
          <p>
            Every Git repository has a <code>.git/hooks</code> folder with a
            script for each hook you can bind to. You're free to change or
            update these scripts as necessary, and Git will execute them when
            those events occur.
          </p>

          <p>Here's a full list of hooks you can attach scripts to:</p>
          <ul>
            <li>
              <a href="https://github.com/git/git/blob/master/templates/hooks--applypatch-msg.sample">applypatch-msg</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/templates/hooks--pre-applypatch.sample">pre-applypatch</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/Documentation/githooks.txt#L74">post-applypatch</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/templates/hooks--pre-commit.sample">pre-commit</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/templates/hooks--prepare-commit-msg.sample">prepare-commit-msg</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/templates/hooks--commit-msg.sample">commit-msg</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/Documentation/githooks.txt#L142">post-commit</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/templates/hooks--pre-rebase.sample">pre-rebase</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/Documentation/githooks.txt#L160">post-checkout</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/Documentation/githooks.txt#L178">post-merge</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/Documentation/githooks.txt#L221">pre-receive</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/templates/hooks--update.sample">update</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/Documentation/githooks.txt#L295">post-receive</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/templates/hooks--post-update.sample">post-update</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/Documentation/githooks.txt#L387">pre-auto-gc</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/Documentation/githooks.txt#L394">post-rewrite</a>
            </li>
            <li>
              <a href="https://github.com/git/git/blob/master/Documentation/githooks.txt#L192">pre-push</a>
            </li>
          </ul>

          <hr class="soften">
          <h2>Why should I care?</h2>
          <p>
            Fair question! Git hooks can greatly increase your productivity as a
            developer. For example, being able to push to your staging or
            production environment without ever leaving Git is just plain
            awesome. Update your code, make a commit and push, and your code can
            be running in any environment you specify. No need to mess with ssh
            or ftp.
          </p>

          <hr class="soften">
          <h2>How do I implement Git hooks?</h2>
          <p>
            The short and easy: Overwrite (or create) one of the scripts in
            <code>.git/hooks</code> and make it executable.
          </p>

          <hr class="soften">
          <h2>Reading</h2>
          <ul>
            <li>
              <a href="http://ryanflorence.com/deploying-websites-with-a-tiny-git-hook/">Deploying websites with a Git hook</a>
            </li>
            <li>
              <a href="http://longair.net/blog/2011/04/09/missing-git-hooks-documentation/">The missing Git hooks documentation</a>
            </li>
            <li>
              <a href="http://omerkatz.com/blog/git-hooks-part-i-the-basics">Git Hooks (Part I): The Basics</a>
            </li>
            <li>
              <a href="http://omerkatz.com/blog/2013/5/23/git-hooks-part-2-implementing-git-hooks-using-python">Git Hooks (Part II): Implementing Git Hooks using Python</a>
            </li>
            <li>
              <a href="http://codeinthehole.com/tips/tips-for-using-a-git-pre-commit-hook/">Tips for using Git pre commit hook</a>
            </li>
            <li>
              <a href="https://wilsonmar.github.io/git-hooks/">Use a boostrap shell script to use Git Hooks in Mac with
                PowerShell and with IntelliJ</a>
            </li>
          </ul>

          <hr class="soften">
          <h2>Projects</h2>
          <ul>
            <li>
              <a href="https://github.com/brigade/overcommit">overcommit</a> - A
              well-maintained, up-to-date, flexible Git hook manager.
            </li>
            <li>
              <a href="https://github.com/mroth/lolcommits">Lolcommits</a> -
              Takes a snapshot with your webcam every time you git commit code,
              and archives a lolcat style image with it.
            </li>
            <li>
              <a href="https://github.com/bmwant/podmena">podmena</a> - Enhance
              your commit messages adding random emoji to it.
            </li>
            <li>
              <a href="https://pre-commit.com/">pre-commit</a> - A framework for
              managing and maintaining multi-language pre-commit hooks.
            </li>
            <li>
              <a href="https://npmjs.org/package/node-hooks">Hooks</a> is a
              command line git hook management tool.
            </li>
            <li>
              <a href="https://github.com/icefox/git-hooks">Git Hooks Manager</a>
              - A tool to manage project, user, and global Git hooks for
              multiple Git repositories.
            </li>
            <li>
              <a href="https://github.com/gnustavo/Git-Hooks">Git::Hooks</a> - A
              framework for implementing Git (and Gerrit) hooks.
            </li>
            <li>
              <a href="https://pypi.python.org/pypi/git-pre-commit-hook">git-pre-commit-hook</a>
              - Hook that blocks bad commits. Useful for Python-development.
            </li>
            <li>
              <a href="https://metacpan.org/pod/App::GitHooks">App::GitHooks</a>
              - A modular and easy to configure git hooks framework, supporting
              <a href="https://metacpan.org/search?q=App%3A%3AGitHooks%3A%3APlugin%3A%3A">many plugins</a>.
            </li>
            <li>
              <a href="https://pythonhosted.org/jig/">Jig</a> - A pre-commit
              hook on steroids
            </li>
            <li>
              <a href="https://github.com/wecodemore/GitPHPHooks">GitPHPHooks</a>
              - Write your hooks in PHP, manage and organize them on a task and
              project level. Has an additional Hooks library
              <a href="https://github.com/wecodemore/GitPHPHooksLibrary">on GitHub</a>
            </li>
            <li>
              <a href="https://github.com/wecodemore/grunt-githooks">Grunt GitHooks</a>
              - Setup, manage and update your hooks with Grunt. Can be used with
              all languages, supports templates.
            </li>
            <li>
              <a href="https://github.com/git-hooks/git-hooks">git-hooks</a> -
              Hook manager.
            </li>
            <li>
              <a href="https://github.com/typicode/husky">Husky</a> - Git hooks
              for Node.js, manage your hooks from your package.json.
            </li>
            <li>
              <a href="https://github.com/BernardoSilva/git-hooks-php">git-hooks-php</a>
              - Git hooks for PHP based projects.
            </li>
            <li>
              <a href="https://github.com/elpete/commandbox-githooks">commandbox-githooks</a>
              - Git hooks for CommandBox CFML based projects.
            </li>
            <li>
              <a href="https://github.com/nkantar/Autohook">Autohook</a> - A
              very, <em>very</em> small Git hook manager with focus on
              automation.
            </li>
            <li>
              <a href="https://pypi.org/project/hooks4git">hooks4git</a> - A
              simple, flexible and language agnostic git hook management
              approach.
            </li>
            <li>
              <a href="https://github.com/rycus86/githooks">Githooks</a> -
              Auto-install Git hook, that supports hooks in any language checked
              into Git and also shared repos.
            </li>
            <li>
              <a href="https://github.com/aitemr/awesome-git-hooks">Awesome Git Hooks</a>
              - A collection of awesome Git Hooks
            </li>
          </ul>
          <hr class="soften">
          <h2>Contribute</h2>
          <p>
            If you have a Git hook you love, or a resource you've written for
            the community - please create a pull request
            <a href="https://github.com/matthewhudson/githooks.com/">here</a>.
          </p>

          <hr class="soften">
          <h2>Maintainer</h2>
          <p>
            Howdy, my name is
            <a href="https://thematthewhudson.com/">Matthew Hudson</a> and I
            created this guide to help myself and others wrap our head around
            integrating Git hooks with WebHooks and WebPipes.
          </p>
        </div>