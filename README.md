# git-LFS

Testing Git LFS, the following steps where performed:

1. Install Git LFS and set it up for the user account
    ```bash
    sudo apt install git-lfs
    git lfs install
    ```
2. Clone the repository
    ```bash
    git clone git@github.com:whordijk/git-LFS.git
    cd git-LFS
    ```
3. Create random large file `data/large_file.dat`
    ```bash
    head -c 1G < /dev/urandom > data/large_file.dat
    ```
4. Track file with git-LFS
    ```bash
    git lfs track data/large_file.dat
    ```
5. Add, commit, and push changes to remote repository
    ```bash
    git add .gitattributes data/large_file.dat
    git commit -m "Track large file with Git LFS"
    git push
    ```

