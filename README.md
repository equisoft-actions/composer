# composer
PHP Composer github action

This action need checkout and php setup
  ```yaml
  steps:
    - name: Checkout
      uses: actions/checkout@v2

    - name: Setup PHP
      uses: shivammathur/setup-php@v2
      with:
        php-version: '7.4'
    - name: Composer install
      uses: equisoft-actions/composer@v1
      with:
        gpr-key: ${{ secrets.gpr-key }}
  ```
