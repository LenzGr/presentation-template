<!-- .slide: data-state="cover" id="dashboard-v2-cover" data-timing="20" -->
<div class="title">
    <h1>Ceph Management and Monitoring with Dashboard V2</h1>
</div>

<div class="row presenters">
    <div class="presenter presenter-1">
        <h3 class="name">Lenz Grimmer</h3>
        <h3 class="job-title">Engineering Team Lead</h3>
        <h3 class="email"><a href="mailto:lgrimmer@suse.com">lgrimmer@suse.com</a></h3>
    </div>
</div>


<!-- .slide: data-state="normal" id="openattic-history" data-timing="20s" data-menu-title="openATTIC History" -->
## openATTIC History

* 2011: openATTIC founded by it-novum
* "Traditional" storage (NAS/SAN): SMB, NFS, iSCSI
* Initial Ceph support added in 2014
* Feb. 2016: Collaboration with SUSE started
* Nov. 2016: openATTIC team joins SUSE
* 2017: oA 3.x focuses on Ceph Management/Monitoring exclusively
  * Salt/DeepSea
  * Prometheus
  * Grafana


<!-- .slide: data-state="normal" id="dashboard-v1" data-timing="20s" data-menu-title="Dashboard v1" -->
## Dashboard v1 Overview

* Added in Ceph Luminous
* Ceph health status, logs, performance metrics
* List of nodes, OSDs
* RBD images, mirroring status, iSCSI daemon status
* Python Backend (CherryPy)
* Javascript UI (Rivets.JS)
* New information added after Luminous
  * RGW details
  * MON list
  * Perf counters
  * Config settings browser


<!-- .slide: data-state="normal" id="dashboard-v1-limitations" data-timing="20s" data-menu-title="Dashboard v1 Limitations" -->
## Dashboard v1 Limitations

* “read-only” - no management functionality
* No built-in authentication system
* Limited functionality of Rivets.JS to create a "real app"
* Intentions to evolve it into a full-blown management and monitoring web UI
  * Wishlist: http://pad.ceph.com/p/mimic-dashboard
  * See “dashboard in mimic” on ceph-devel - https://marc.info/?l=ceph-devel&m=151376737304374
  * Sage during the Dec. 2017 CDM call: https://youtu.be/YNfp_4S7mYE?t=28m37s


<!-- .slide: data-state="normal" id="dashboard-v2-history" data-timing="20s" data-menu-title="Dashboard v2 History" -->
## Dashboard v2 History

* Jan. 2018: Initial discussions with Sage and John
* POC of a Ceph Mgr Dashboard converted to Angular
  * http://pad.ceph.com/p/ceph-dashboard-angular-prototype
  * https://github.com/tspmelo/ceph/tree/ceph-dashboard-angular/
* Feb. 22nd 2018: Dashboard v2 development branch created
  * https://github.com/openattic/ceph/tree/wip-mgr-dashboard_v2
* Milestone 1 (Dashboard v1 feature parity) merged on 2018-03-06
  * https://github.com/ceph/ceph/pull/20103


<!-- .slide: data-state="normal" id="dashboard-v2-overview" data-timing="20s" data-menu-title="Dashboard v2 Overview" -->
## Dashboard v2 Overview

* Modular Python backend (CherryPy), RESTful API
* WebUI (Angular 5), inspired by / derived from openATTIC UI
* Basic username/password authentication
* All features of Dashboard v1 from current `master` branch


<!-- .slide: data-state="normal" id="nested-lists" data-timing="20s" data-menu-title="Next Steps" -->
## Next Steps

### Reaching feature parity with openATTIC 3.x

* RBD management (create/modify/delete)
* RGW management (create/modify/delete users, keys, buckets)
* Ceph Pool management (create/modify/delete)
* SSL/TLS support
* Embedded Grafana Dashboards
* iSCSI target management (TCMU runner)
* NFS Ganesha management