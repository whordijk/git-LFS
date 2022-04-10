# git-LFS

Testing git-LFS, the following steps where performed:

1. Install git-LFS
    ```bash
    sudo apt install git-lfs
    ```
2. Clone the repository
    ```bash
    git clone git@github.com:whordijk/git-LFS.git
    ```
3. Create random large file`data/large_file.dat`
    ```bash
    head -c 1G </dev/urandom >data/large_file.dat
    ```
4. Track file with git-LFS
    ```bash
    git lfs track data/large_file.dat
    ```
5. Push to remote repository
    ```bash
    git add .
    git commit -m "Initialize git LFS file tracking"
    git push
    ```

