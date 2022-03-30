# Configuring Git/Blot

Clone this repo etc.

Now go into your `.git/config` file. Make sure the following is set:
```
[remote "origin"]
	url = git@github.com:suspendedreason/tis-so.git
	fetch = +refs/heads/*:refs/remotes/origin/*
	pushurl = git@github.com:suspendedreason/tis-so.git
	pushurl = https://blot.im/clients/git/end/tis.git
```

This will ensure that `git push` dispatches to both the Blot site and the GH repo.

# Posting

To queue a post, name it after the next-soonest available date.

For some reason TBD, the standard naming system does not suffice for scheduling, so add a date manually at the top of the post.

Metadata format:
```
Date: YYYYMMDD
Tags: separated by commas, lowercase, Except For Proper Nouns
```

When adding assets, include an underscore before the file name to prevent their being listed on the blog as a discrete post.

Any Tweets, similar content that may be deleted/taken down, try to back it up with a screenshot!

Wikilinks are formatted with [[double brackets]] e.g. [[220329]]. Backlinks will happen automatically. You can rename via [[Other post|Link text]].