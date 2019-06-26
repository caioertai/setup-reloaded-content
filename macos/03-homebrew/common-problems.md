* If you get a `/usr/local must be writable` error when running `brew update`, run this:

    ```bash
    sudo chown -R $USER:admin /usr/local
    brew update
    ```
