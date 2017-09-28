# enchepan
Ceph iSCSI using LRBD

Steps :
1. Deploy ceph on fedora/centos/rhel node using `ceph-deploy`
2. Copy `ceph.conf` and keyring from existing node to `/etc/ceph`
3. Install all rpm on `rpm` folder
4. Create lrbd config or use `simple.json` that included on `lrbd` folder as baseline.
5. Run lrbd -f `simple.json` followed by `lrbd -H "hostname"`
6. Check whether the target has been made using `targetcli ls`
