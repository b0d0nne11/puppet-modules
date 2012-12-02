# Puppet module for ruby-build

> "ruby-build is an rbenv plugin that provides an rbenv install command to
compile and install different versions of Ruby on UNIX-like systems."
  ~ https://github.com/sstephenson/ruby-build

## Basic Usage

To install ruby-build

    class { 'ruby_build': }

## Resource

To install a ruby version

    ruby_build::resource::ruby { '1.9.3-p327': }

To install a gem

    ruby_build::resource::gem  { 'bundler':
      gem_version => '1.2.3',
      ruby_name   => '1.9.3-p327'
    }

## License

Copyright (C) 2012 Brendan O'Donnell

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.