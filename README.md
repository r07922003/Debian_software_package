show how to package the debian software

dh_make -p myhello_1.0 --createorig

cd debian/

rm *.ex *.EX

git add debian/

git commit -m "Towards a debian package"

gbp buildpackage --git-ignore-new


sudo add-apt-repository ppa:nealson840123/hellow

