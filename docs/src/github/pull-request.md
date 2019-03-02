<style>div{direction:rtl;float:right;} .intro{bachground-color:#ccc;}</style>

##ایجاد Pull request

<div class='intro'>
<p>Create a pull request to propose and collaborate on changes to a repository. These changes are proposed in a <em>branch</em>, which ensures that the <code>master</code> branch only contains finished and approved work.</p>
</div>
<p>Pull requests can only be opened if there are differences between your branch and the upstream branch. You can specify which branch you'd like to merge your changes into when you create your pull request.</p>

<p>If you don't have write access to the repository where you'd like to create a pull request, you must create a fork, or copy, of the repository first. For more information, see "<a href="/articles/creating-a-pull-request-from-a-fork">Creating a pull request from a fork</a>" and "<a href="/articles/about-forks">About forks</a>."</p>

<div class="alert note">

<p><strong>Note</strong>: To open a pull request in a public repository, you must have write access to the head or the source branch or, for organization-owned repositories, you must be a member of the organization that owns the repository to open a pull request.</p>

</div>

<p>You can close corresponding issues using a keyword in your pull request or commit message. For more information, see "<a href="/articles/closing-issues-using-keywords">Closing issues using keywords</a>."</p>

<h3>
<a id="changing-the-branch-range-and-destination-repository" class="anchor" href="#changing-the-branch-range-and-destination-repository" aria-hidden="true"><span aria-hidden="true" class="octicon octicon-link"></span></a>Changing the branch range and destination repository</h3>

<p>By default, pull requests are based on the parent repository's <a href="/articles/setting-the-default-branch">default branch</a>.</p>

<p>If the default parent repository isn't correct, you can change both the parent repository and the branch with the drop-down lists. You can also swap your head and base branches with the drop-down lists to establish diffs between reference points. References here must be branch names in your GitHub repository.</p>

<p><img src="/assets/images/help/pull_requests/pull-request-review-edit-branch.png" alt="Pull Request editing branches"></p>

<p>When thinking about branches, remember that the <em>base branch</em> is <strong>where</strong> changes should be applied, the <em>head branch</em> contains <strong>what</strong> you would like to be applied.</p>

<p>When you change the base repository, you also change notifications for the pull request. Everyone that can push to the base repository will receive an email notification and see the new pull request in their dashboard the next time they sign in.</p>

<p>When you change any of the information in the branch range, the Commit and Files changed preview areas will update to show your new range.</p>

<div class="alert tip">

<p><strong>Tips</strong>:</p>

<ul>
<li>Using the compare view, you can set up comparisons across any timeframe. For more information, see "<a href="/articles/comparing-commits-across-time">Comparing commits across time</a>."</li>
<li>Project maintainers can add a pull request template for a repository. Templates include prompts for information in the body of a pull request. For more information, see "<a href="/articles/about-issue-and-pull-request-templates">About issue and pull request templates</a>."</li>
</ul>

</div>

<h3>
<a id="creating-the-pull-request" class="anchor" href="#creating-the-pull-request" aria-hidden="true"><span aria-hidden="true" class="octicon octicon-link"></span></a>Creating the pull request</h3>

<ol>
<li><p>On GitHub, navigate to the main page of the repository.</p></li>
<li><p>In the "Branch" menu, choose the branch that contains your commits.
<img src="/assets/images/help/pull_requests/branch-dropdown.png" alt="Branch dropdown menu"></p></li>
<li><p>To the right of the Branch menu, click <strong>New pull request</strong>.
<img src="/assets/images/help/pull_requests/pull-request-start-review-button.png" alt="Pull Request button"></p></li>
<li><p>Use the <em>base</em> branch dropdown menu to select the branch you'd like to merge your changes into, then use the <em>compare</em> branch drop-down menu to choose the topic branch you made your changes in.
<img src="/assets/images/help/pull_requests/choose-base-and-compare-branches.png" alt="Drop-down menus for choosing the base and compare branches"></p></li>
<li><p>Type a title and description for your pull request.
<img src="/assets/images/help/pull_requests/pullrequest-description.png" alt="Pull request title and description fields"></p></li>
<li><p>Click <strong>Create pull request</strong>.
<img src="/assets/images/help/pull_requests/pullrequest-send.png" alt="Create pull request button"></p></li>
</ol>

<div class="alert tip">

<p><strong>Tip:</strong> After you create a pull request, you can ask a specific person to <a href="/articles/reviewing-proposed-changes-in-a-pull-request">review your proposed changes</a>. For more information, see "<a href="/articles/requesting-a-pull-request-review">Requesting a pull request review</a>."</p>

</div>

<p>After your pull request has been reviewed, it can be <a href="/articles/merging-a-pull-request">merged into the repository</a>.</p>

<h3>
<a id="further-reading" class="anchor" href="#further-reading" aria-hidden="true"><span aria-hidden="true" class="octicon octicon-link"></span></a>Further reading</h3>

<ul>
<li>"<a href="/articles/creating-a-pull-request-from-a-fork">Creating a pull request from a fork</a>"</li>
<li>"<a href="/articles/changing-the-base-branch-of-a-pull-request">Changing the base branch of a pull request</a>"</li>
<li>"<a href="/articles/adding-issues-and-pull-requests-to-a-project-board/#adding-issues-and-pull-requests-to-a-project-board-from-the-sidebar">Adding issues and pull requests to a project board from the sidebar</a>"</li>
</ul>
        </div>

        <div class="support-footer">
  <ul class="article-footer button-nav">
    
      <li><a href="https://github.com/contact" class="minibutton" onClick="_gaq.push(['_trackEvent', 'Contact Support', 'Creating a pull request', window.location.href]);">
          <span class="octicon octicon-comment-discussion"></span>
          Contact a human
        </a>
      </li>
    
  </ul>
</div>

