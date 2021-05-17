```sh
brew install virtualbox --cask
brew install vagrant --cask
```
セキュリティ・プライバシーについて確認を求められた場合は許可。
brew で入れられない場合は dmg をダウンロード。
https://www.vagrantup.com/downloads

windows の virtual machine をダウンロード。
https://developer.microsoft.com/ja-jp/microsoft-edge/tools/vms/

```sh
unzip ~/Downloads/MSEdge.Win10.Vagrant.zip
vagrant box add MSEdge\ -\ Win10.box --name win10
```
```sh
vagrant up
```
