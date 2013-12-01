yasnippet-ruby-mode
===================

Comprehensive collection of Ruby snippets for yasnippet. Includes snippets for Rails and RSpec.

To use this via el-get, start with this recipe:

	(:name yasnippet-ruby-mode
	       :website "https://github.com/pedz/yasnippet-ruby-mode"
	       :Description "Comprehensive collection of Ruby snippets for yasnippet. Includes snippets for Rails and RSpec."
	       :type github
	       :pkgname "pedz/yasnippet-ruby-mode"
	       :branch "rearranged"
	       :post-init (eval-after-load 'yasnippet
			    '(progn
			       (message "adding ruby mode to snippets")
			       (add-to-list 'yas-snippet-dirs
					    (concat el-get-dir (file-name-as-directory "yasnippet-ruby-mode"))))))
