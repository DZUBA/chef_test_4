# chef_test_4

First of all I've installed packer by https://www.packer.io/downloads.html
Than I've get to Microsoft site to get newest iso of Windows Server 2012R2.
In this task I've used mwrock's repo https://github.com/mwrock/packer-templates
Here I've changed path to my iso https://github.com/DZUBA/chef_test_4/blob/master/vbox-2012r2.json#L96
To decline Windows updates I've commented this line https://github.com/DZUBA/chef_test_4/blob/master/scripts/package.ps1#L8
Build process starts with command
```
packer build -only virtualbox-iso .\vbox-2012r2.json
```

Q: What is packer?

A: Packer is a tool which helps to create images with using systems of configuration management. It also helps to automated process of creating with freshest soft where and packages.

Q: Why you can’t download windows boxes from the Internet?

A: Probably because of Microsoft license processes.

Q: What is used for preparing box by packer?

A: Because it's fully automated process, where as result you'll receive golden image with fresh soft and packages.

Q: Time for preparing Win2012r2 box with updates?

A: At my sandbox machine it took almost 11 hours

Q: Time for preparing Win2012r2 box without updates?

A: Less than two hours.
