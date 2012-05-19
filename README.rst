RFC Syntax
==========

NOTE
----
This is only a mirror of `vim script`_. I created this because the `vim-scripts mirror on github`_ doesn't include this plugin.

:Authors:
    lilydjwg

:Version:
    1.0
 
:Script Type:
    syntax
 
Description
-----------
Simple syntax highlight for RFC (Request For Comments) file. 
It can highlight the contents, the titles and so on. 

A ftplugin is also provided to use <C-]> to jump from the contents or reference note ([1] like things). You can then use <C-t> to go back (once only). <C-o> and `` should work as expected.
 
Install Details
---------------
unzip the archive to your .vim (or vimfiles) directory. 
You must add filetype detect by yourself. For example, add 

  if expand('%:t') =~? 'rfc\d\+' 
    setfiletype rfc 
  endif 

to your scripts.vim will make Vim recognize all files with name rfcXXXX as RFC file. 

.. _vim script: http://www.vim.org/scripts/script.php?script_id=2930
.. _vim-scripts mirror on github: https://github.com/vim-scripts
