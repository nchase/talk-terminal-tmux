_The_ Source of Sadness In Software Engineering:
------------------------------------------------
* Slow feedback. <span class="fragment">"I'm working...<span class="fragment">but I don't know if what I'm working on is working."</span></span>
* Manifestations: <!-- .element: class="fragment" style="visibility: hidden;" -->
	<!-- * <li class="fragment">"Where am I again?"</li><li class="fragment">Who are you?</li><!-- .element class="fragment" style="visibility: hidden;" --> -->



Make Your Machine Work For You.
-------------------------------



Terminal improvements for fun and profit*
-----------------------------------------

<br/>

<small class="fragment small">
	*Where 'profit' is increased productivity, gratification, and radical self-actualization.
</small>

<br/>

<small style="display: block;">Noah Chase [<a style="line-height: inherit;" href="http://twitter.com/nchase">@nchase</a>]</small>



Assumptions:
------------

* "My environment can be improved. <br/> <span style="padding-left: 120px;"></span> I can improve my environment."
* "If I take time to improve my environment, I will become faster." <!-- .element: class="fragment" -->
* "I can afford to invest time in improving my environment." <!-- .element: class="fragment" -->



Core needs:
-----------

1. Prompt must display cwd                             <!-- .element: class="fragment nolist" -->
	- ![/images/00-00-cwd.png](/images/00-00-cwd.png)    <!-- .element: class="fragment" -->
2. Prompt must display current git branchname          <!-- .element: class="fragment nolist" -->
	- ![/images/00-01-git-branch.png](/images/00-01-git-branch.png)    <!-- .element: class="fragment" -->
3. Prompt must have git branch autocompletion          <!-- .element: class="fragment nolist" -->
	- ![/images/00-01-git-completion.png](/images/00-01-git-completion.png)    <!-- .element: class="fragment" -->



<!-- empty slide -->


<!-- spinning dollar signs. -->

<i class="fa fa-usd fa-spin"></i> <i class="fa fa-usd fa-spin"></i> <i class="fa fa-usd fa-spin"></i>
-----------

![/images/00-00-icing.png](/images/00-00-icing.png)    <!-- .element: class="fragment" -->



Terminal Processes
------------------

![/images/03-00-terminals.png](/images/03-00-terminals.png)    <!-- .element: class="fragment" -->

1. How do you distinguish between them? <!-- .element: class="fragment" -->
2. How do you find the one you need quickly? <!-- .element: class="fragment" -->
3. Can you 'drop it all on the floor'? <!-- .element: class="fragment" -->
4. How do you keep it all in your head? <!-- .element: class="fragment" -->



Terminal Multiplexing:
----------------------

0. Electronics: 'Multiple signals sharing one resource'
1. <!-- .element: class="fragment" --> See `screen` [incep. 1987], `tmux` [incep. 2009]
2. Literally run infinite programs in a single terminal instance (if you want to) <!-- .element: class="fragment" -->
	- 'session' persists when terminal is closed &mdash; processes still run <!-- .element: class="fragment" -->
	- a session can have many 'windows', containing shells or processes <!-- .element: class="fragment" -->
3. Issue commands to your shell as normal. <!-- .element: class="fragment" -->



Terminal Multiplexing, Cont.
----------------------------

4. Issue commands to multiplexer with a 'prefix' sequence
	* windows: 'next', 'previous', 'create', 'rename' <!-- .element: class="fragment" -->
	* sessions: 'show', 'rename' <!-- .element: class="fragment" -->
	* <!-- .element: class="fragment" --> `tmux attach -t {sessionname}` 



`tmuxinator`: tmux for projects
-------------------------------

1. "Manage complex tmux sessions easily" - https://github.com/tmuxinator/tmuxinator
2. start everything you need for a repo, project, etc in a single command - generate all of the context you need to work on a project. <!-- .element: class="fragment" -->
	* e.g. `tmuxinator webs`
3. Just detach it or close the window when you're done, re-attach it later. Maybe you need to work on another project/repo? <!-- .element: class="fragment" -->



<!-- empty slide -->
