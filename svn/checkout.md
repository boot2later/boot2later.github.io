# svn checkout
 
## Make an empty checkout of the repository:
checkout empty repo from `https://github.com/boot2later/boot2later.github.io.git`

	svn checkout --depth empty https://github.com/boot2later/boot2later.github.io

## Get the `trunk` branch
The Subversion bridge maps `trunk` to the Git HEAD branch (which is usually `master`).
	svn up trunk

## Get an empty checkout of the branches directory.
This is where all of the non-HEAD branches live, and where you'll be making feature branches.

	svn up --depth empty branches

## Creating branches

	svn copy trunk/ branches/svn_demo

## commit branch

	svn commit -m 'Added svn_demo topic branch'

## status 

	svn status 

