# git

# git ls-tree HEAD
100644 blob 55c0287d4ef21f15b97eb1f107451b88b479bffe    script.sh
As you can see the file has 644 permission (ignoring the 100). We would like to change it to 755:

# git update-index --chmod=+x script.sh
commit the changes

# git commit -m "Changing file permissions"
[master 77b171e] Changing file permissions
0 files changed, 0 insertions(+), 0 deletions(-)
mode change 100644 => 100755 script.sh


git push
