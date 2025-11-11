# infra-terraform
# ==============

"""
infra-terraform: a terraform module for infrastructure as code
===========================================================

This module provides a set of terraform resources and modules for managing
infrastructure as code.

"""

from setuptools import setup

setup(
    name='infra-terraform',
    version='1.0.0',
    packages=['infra_terraform'],
    install_requires=[
        'terraform==1.1.3',
        'toml==0.10.2'
    ],
    entry_points={
        'console_scripts': ['infra-terraform=infra_terraform.main:main']
    }
)