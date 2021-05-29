
name: Python package

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  build:

    runs-on: ubuntu-latest
    strategy:
      fail-fast: false
      matrix:
        python-version: [3.7, 3.8, 3.9]

    steps:
    - uses: actions/checkout@v2
    - name: Set up Python ${{ matrix.python-version }}
      uses: actions/setup-python@v2
      with:
        python-version: ${{ matrix.python-version }}
    - name: Install dependencies
      run: |
        python -m pip install --upgrade pip
        python -m pip install flake8 pytest
        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
    - name: Lint with flake8
      run: |
        # stop the build if there are Python syntax errors or undefined names
        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
    - name: Test with pytest
      run: - name: EKS on Fargate
  uses: aws-actions/amazon-eks-fargate@v0.1.1
- name: AWS CloudFormation "Deploy CloudFormation Stack" Action for GitHub Actions
  uses: aws-actions/aws-cloudformation-github-deploy@v1.0.3

        pytest: Super-Ghcz-master
 >
- git@github.com:INOS-soft/The-Journey-0.60sec-atom.git
- git@github.com:INOS-soft/Express-Helpers.git
- git@github.com:INOS-soft/hyperHTML-Magic-INOS_soft.git
- git@github.com:hugo53/awesome-RemoteWork.git
- git@github.com:INOS-soft/GitHub.git
- git@github.com:INOS-soft/virtual-environments-forge-ultralite.git
- git@github.com:wyattowalsh/wyattowalsh.git
