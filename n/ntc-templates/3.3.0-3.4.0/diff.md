# Comparing `tmp/ntc_templates-3.3.0.tar.gz` & `tmp/ntc_templates-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntc_templates-3.3.0.tar", max compression
+gzip compressed data, was "ntc_templates-3.4.0.tar", max compression
```

## Comparing `ntc_templates-3.3.0.tar` & `ntc_templates-3.4.0.tar`

### file list

```diff
@@ -1,584 +1,592 @@
--rw-r--r--   0        0        0      601 2023-03-21 20:38:25.436750 ntc_templates-3.3.0/LICENSE
--rw-r--r--   0        0        0     2842 2023-03-21 20:38:25.436750 ntc_templates-3.3.0/README.md
--rw-r--r--   0        0        0      260 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/__init__.py
--rw-r--r--   0        0        0     2180 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/parse.py
--rw-r--r--   0        0        0      700 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm
--rw-r--r--   0        0        0      170 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_oam_mac-ping.textfsm
--rw-r--r--   0        0        0      371 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_lag.textfsm
--rw-r--r--   0        0        0      641 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_port.textfsm
--rw-r--r--   0        0        0      434 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_bgp_routes_vpn-ipv4.textfsm
--rw-r--r--   0        0        0      526 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm
--rw-r--r--   0        0        0      662 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm
--rw-r--r--   0        0        0      318 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_isis_adjacency.textfsm
--rw-r--r--   0        0        0      336 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_isis_interface.textfsm
--rw-r--r--   0        0        0      619 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm
--rw-r--r--   0        0        0      608 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm
--rw-r--r--   0        0        0      512 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm
--rw-r--r--   0        0        0      547 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm
--rw-r--r--   0        0        0      425 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_pim_interface.textfsm
--rw-r--r--   0        0        0      649 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm
--rw-r--r--   0        0        0      544 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm
--rw-r--r--   0        0        0      665 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm
--rw-r--r--   0        0        0      598 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm
--rw-r--r--   0        0        0      642 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm
--rw-r--r--   0        0        0      522 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm
--rw-r--r--   0        0        0      371 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_bash_df_-h.textfsm
--rw-r--r--   0        0        0      430 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_dir_flash.textfsm
--rw-r--r--   0        0        0      121 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_boot-config.textfsm
--rw-r--r--   0        0        0      226 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_clock.textfsm
--rw-r--r--   0        0        0      524 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm
--rw-r--r--   0        0        0      525 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm
--rw-r--r--   0        0        0      107 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_hostname.textfsm
--rw-r--r--   0        0        0      878 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm
--rw-r--r--   0        0        0      427 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      399 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      313 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver.textfsm
--rw-r--r--   0        0        0      757 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm
--rw-r--r--   0        0        0      666 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_inventory.textfsm
--rw-r--r--   0        0        0      517 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm
--rw-r--r--   0        0        0      159 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_arp.textfsm
--rw-r--r--   0        0        0      651 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm
--rw-r--r--   0        0        0     1568 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0      246 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_helper-address.textfsm
--rw-r--r--   0        0        0      169 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      736 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm
--rw-r--r--   0        0        0      387 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      462 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      734 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm
--rw-r--r--   0        0        0     1035 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm
--rw-r--r--   0        0        0     1101 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm
--rw-r--r--   0        0        0      358 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_isis_neighbors.textfsm
--rw-r--r--   0        0        0      190 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      627 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1662 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      257 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_mac_security_interface.textfsm
--rw-r--r--   0        0        0      303 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_mac_security_mka_counters.textfsm
--rw-r--r--   0        0        0     1431 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm
--rw-r--r--   0        0        0      279 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_mlag.textfsm
--rw-r--r--   0        0        0      716 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_module.textfsm
--rw-r--r--   0        0        0      557 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm
--rw-r--r--   0        0        0      403 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_pim_ipv4_neighbor.textfsm
--rw-r--r--   0        0        0     1222 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm
--rw-r--r--   0        0        0     5405 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm
--rw-r--r--   0        0        0      573 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm
--rw-r--r--   0        0        0      275 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_snmp_community.textfsm
--rw-r--r--   0        0        0      424 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_version.textfsm
--rw-r--r--   0        0        0     6187 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_vlan.textfsm
--rw-r--r--   0        0        0     4153 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_vrf.textfsm
--rw-r--r--   0        0        0      701 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm
--rw-r--r--   0        0        0      322 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_arp_all-vrfs.textfsm
--rw-r--r--   0        0        0      596 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm
--rw-r--r--   0        0        0      531 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm
--rw-r--r--   0        0        0      531 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm
--rw-r--r--   0        0        0     2201 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm
--rw-r--r--   0        0        0     4761 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm
--rw-r--r--   0        0        0      348 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_ip_route_all-vrfs.textfsm
--rw-r--r--   0        0        0      827 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm
--rw-r--r--   0        0        0      240 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_mac-address-table.textfsm
--rw-r--r--   0        0        0      380 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_ntp_associations.textfsm
--rw-r--r--   0        0        0      662 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm
--rw-r--r--   0        0        0      917 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm
--rw-r--r--   0        0        0      768 2023-03-21 20:38:25.440750 ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm
--rw-r--r--   0        0        0     1028 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm
--rw-r--r--   0        0        0      977 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm
--rw-r--r--   0        0        0      735 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_arp.textfsm
--rw-r--r--   0        0        0      176 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      287 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      119 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_interface_name.textfsm
--rw-r--r--   0        0        0      702 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm
--rw-r--r--   0        0        0      181 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_mac-address-table.textfsm
--rw-r--r--   0        0        0      878 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm
--rw-r--r--   0        0        0      607 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm
--rw-r--r--   0        0        0     1825 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm
--rw-r--r--   0        0        0      470 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_vlan.textfsm
--rw-r--r--   0        0        0      367 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/avaya_vsp_show_software.textfsm
--rw-r--r--   0        0        0      583 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm
--rw-r--r--   0        0        0      631 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm
--rw-r--r--   0        0        0      458 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/broadcom_icos_show_mac-addr-table.textfsm
--rw-r--r--   0        0        0     1497 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/broadcom_icos_show_version.textfsm
--rw-r--r--   0        0        0      372 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/broadcom_icos_show_vlan_brief.textfsm
--rw-r--r--   0        0        0      358 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_arp.textfsm
--rw-r--r--   0        0        0     5683 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm
--rw-r--r--   0        0        0      695 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      367 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_lag_brief.textfsm
--rw-r--r--   0        0        0      416 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      906 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      375 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_mac-address.textfsm
--rw-r--r--   0        0        0     1120 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm
--rw-r--r--   0        0        0      301 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_monitor.textfsm
--rw-r--r--   0        0        0     2278 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm
--rw-r--r--   0        0        0      851 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm
--rw-r--r--   0        0        0      351 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_topo.textfsm
--rw-r--r--   0        0        0     2990 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm
--rw-r--r--   0        0        0     1629 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm
--rw-r--r--   0        0        0     6614 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm
--rw-r--r--   0        0        0      430 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      367 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_lag_brief.textfsm
--rw-r--r--   0        0        0      906 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1071 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm
--rw-r--r--   0        0        0      311 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_monitor_actual.textfsm
--rw-r--r--   0        0        0     1618 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm
--rw-r--r--   0        0        0     2277 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm
--rw-r--r--   0        0        0      739 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_span.textfsm
--rw-r--r--   0        0        0      591 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm
--rw-r--r--   0        0        0      167 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_fw_stat.textfsm
--rw-r--r--   0        0        0      170 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_arp_dynamic_all.textfsm
--rw-r--r--   0        0        0      148 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_asset_all.textfsm
--rw-r--r--   0        0        0      189 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_dns.textfsm
--rw-r--r--   0        0        0       71 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_domainname.textfsm
--rw-r--r--   0        0        0      786 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm
--rw-r--r--   0        0        0      482 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_ipv6_route.textfsm
--rw-r--r--   0        0        0      159 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_lom.textfsm
--rw-r--r--   0        0        0      208 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_ntp_servers.textfsm
--rw-r--r--   0        0        0      550 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm
--rw-r--r--   0        0        0      236 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_version_all.textfsm
--rw-r--r--   0        0        0      419 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_chassis_show_temperature.textfsm
--rw-r--r--   0        0        0     1010 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_port_show.textfsm
--rw-r--r--   0        0        0      945 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm
--rw-r--r--   0        0        0      623 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_software_show.textfsm
--rw-r--r--   0        0        0      289 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_ssh_server_show_key.textfsm
--rw-r--r--   0        0        0      556 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm
--rw-r--r--   0        0        0      636 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm
--rw-r--r--   0        0        0      714 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm
--rw-r--r--   0        0        0      663 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_dir.textfsm
--rw-r--r--   0        0        0      661 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_ping.textfsm
--rw-r--r--   0        0        0     4925 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm
--rw-r--r--   0        0        0      325 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_arp.textfsm
--rw-r--r--   0        0        0     9761 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm
--rw-r--r--   0        0        0      829 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm
--rw-r--r--   0        0        0     1377 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm
--rw-r--r--   0        0        0      917 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm
--rw-r--r--   0        0        0      438 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_crypto_ikev1_sa_detail.textfsm
--rw-r--r--   0        0        0     6136 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm
--rw-r--r--   0        0        0     3036 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_failover.textfsm
--rw-r--r--   0        0        0     4402 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_interface.textfsm
--rw-r--r--   0        0        0     7080 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm
--rw-r--r--   0        0        0      268 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_interface_ip_brief.textfsm
--rw-r--r--   0        0        0      320 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_inventory.textfsm
--rw-r--r--   0        0        0     4240 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm
--rw-r--r--   0        0        0     2352 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_logging.textfsm
--rw-r--r--   0        0        0       89 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_name.textfsm
--rw-r--r--   0        0        0     1624 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_nat.textfsm
--rw-r--r--   0        0        0      561 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm
--rw-r--r--   0        0        0      403 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      374 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_ospf_neighbor.textfsm
--rw-r--r--   0        0        0     1208 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm
--rw-r--r--   0        0        0      425 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_resource_usage.textfsm
--rw-r--r--   0        0        0     1606 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_route.textfsm
--rw-r--r--   0        0        0     2300 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm
--rw-r--r--   0        0        0      437 2023-03-21 20:38:25.444750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_ikev1.textfsm
--rw-r--r--   0        0        0     1212 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm
--rw-r--r--   0        0        0     1726 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm
--rw-r--r--   0        0        0      474 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_object_network.textfsm
--rw-r--r--   0        0        0     4906 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm
--rw-r--r--   0        0        0      967 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_version.textfsm
--rw-r--r--   0        0        0     1625 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm
--rw-r--r--   0        0        0     1822 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm
--rw-r--r--   0        0        0     7479 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm
--rw-r--r--   0        0        0     1126 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm
--rw-r--r--   0        0        0      481 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_dir.textfsm
--rw-r--r--   0        0        0      859 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_ping.textfsm
--rw-r--r--   0        0        0     1470 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm
--rw-r--r--   0        0        0      416 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_access-session.textfsm
--rw-r--r--   0        0        0      953 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm
--rw-r--r--   0        0        0      355 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_alert_counters.textfsm
--rw-r--r--   0        0        0      310 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_aliases.textfsm
--rw-r--r--   0        0        0      523 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm
--rw-r--r--   0        0        0      615 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_archive.textfsm
--rw-r--r--   0        0        0      403 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_authentication_sessions.textfsm
--rw-r--r--   0        0        0     2496 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm
--rw-r--r--   0        0        0     1700 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_boot.textfsm
--rw-r--r--   0        0        0      264 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_capability_feature_routing.textfsm
--rw-r--r--   0        0        0      538 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm
--rw-r--r--   0        0        0      937 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      317 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_clock.textfsm
--rw-r--r--   0        0        0     2327 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm
--rw-r--r--   0        0        0     6120 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm
--rw-r--r--   0        0        0     2126 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm
--rw-r--r--   0        0        0     1418 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm
--rw-r--r--   0        0        0     1041 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm
--rw-r--r--   0        0        0      491 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_dmvpn.textfsm
--rw-r--r--   0        0        0     1367 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm
--rw-r--r--   0        0        0      413 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_environment_power_all.textfsm
--rw-r--r--   0        0        0     1603 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm
--rw-r--r--   0        0        0     1188 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm
--rw-r--r--   0        0        0      454 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_hosts_summary.textfsm
--rw-r--r--   0        0        0     1226 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm
--rw-r--r--   0        0        0      312 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interface_transceiver.textfsm
--rw-r--r--   0        0        0     2668 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm
--rw-r--r--   0        0        0      409 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      898 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm
--rw-r--r--   0        0        0     1512 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm
--rw-r--r--   0        0        0      570 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm
--rw-r--r--   0        0        0     2587 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm
--rw-r--r--   0        0        0      525 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm
--rw-r--r--   0        0        0     2029 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm
--rw-r--r--   0        0        0     1706 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm
--rw-r--r--   0        0        0     2011 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm
--rw-r--r--   0        0        0      589 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0     1761 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm
--rw-r--r--   0        0        0     1207 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm
--rw-r--r--   0        0        0     3244 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm
--rw-r--r--   0        0        0      711 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm
--rw-r--r--   0        0        0     2669 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm
--rw-r--r--   0        0        0      773 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm
--rw-r--r--   0        0        0     2597 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm
--rwxr-xr-x   0        0        0      459 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_flow_toptalkers.textfsm
--rw-r--r--   0        0        0     4260 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm
--rw-r--r--   0        0        0     1909 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm
--rw-r--r--   0        0        0      288 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0     1378 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm
--rw-r--r--   0        0        0      645 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm
--rw-r--r--   0        0        0      778 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm
--rw-r--r--   0        0        0     1362 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm
--rw-r--r--   0        0        0     1807 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm
--rw-r--r--   0        0        0      396 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      383 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      436 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_prefix-list.textfsm
--rw-r--r--   0        0        0     2496 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm
--rw-r--r--   0        0        0     1389 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm
--rw-r--r--   0        0        0      555 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm
--rw-r--r--   0        0        0      472 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_vrf_interfaces.textfsm
--rw-r--r--   0        0        0      917 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm
--rw-r--r--   0        0        0      399 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      371 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      523 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm
--rw-r--r--   0        0        0      956 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm
--rw-r--r--   0        0        0      412 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_isis_neighbors.textfsm
--rw-r--r--   0        0        0      547 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_license.textfsm
--rw-r--r--   0        0        0      479 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0     2344 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     5593 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_logging.textfsm
--rw-r--r--   0        0        0     4086 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm
--rw-r--r--   0        0        0     1017 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_module.textfsm
--rw-r--r--   0        0        0      585 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm
--rw-r--r--   0        0        0     1062 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm
--rw-r--r--   0        0        0      760 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm
--rw-r--r--   0        0        0      350 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_mpls_interfaces.textfsm
--rw-r--r--   0        0        0      377 2023-03-21 20:38:25.448750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_nve_peers.textfsm
--rw-r--r--   0        0        0      346 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_nve_vni.textfsm
--rw-r--r--   0        0        0     1215 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm
--rw-r--r--   0        0        0     1072 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm
--rw-r--r--   0        0        0      974 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm
--rw-r--r--   0        0        0      922 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm
--rw-r--r--   0        0        0      684 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm
--rw-r--r--   0        0        0      314 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_power_supplies.textfsm
--rw-r--r--   0        0        0      344 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_processes_cpu.textfsm
--rw-r--r--   0        0        0      640 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm
--rw-r--r--   0        0        0     3950 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm
--rw-r--r--   0        0        0      784 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm
--rw-r--r--   0        0        0     3318 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm
--rw-r--r--   0        0        0     1034 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm
--rw-r--r--   0        0        0      359 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_snmp_community.textfsm
--rw-r--r--   0        0        0      802 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm
--rw-r--r--   0        0        0      668 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm
--rw-r--r--   0        0        0      413 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_spanning-tree.textfsm
--rw-r--r--   0        0        0     2018 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_standby.textfsm
--rw-r--r--   0        0        0      621 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm
--rw-r--r--   0        0        0      495 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_switch_detail.textfsm
--rw-r--r--   0        0        0      357 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_switch_detail_stack_ports.textfsm
--rw-r--r--   0        0        0     1009 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm
--rw-r--r--   0        0        0     1735 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_version.textfsm
--rw-r--r--   0        0        0     6327 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm
--rw-r--r--   0        0        0      534 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm
--rw-r--r--   0        0        0     1596 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm
--rw-r--r--   0        0        0     1655 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm
--rw-r--r--   0        0        0     1109 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm
--rw-r--r--   0        0        0     1660 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_traceroute.textfsm
--rw-r--r--   0        0        0     1548 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm
--rw-r--r--   0        0        0      461 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors.textfsm
--rw-r--r--   0        0        0      689 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      203 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_clock.textfsm
--rw-r--r--   0        0        0      210 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_configuration_session_summary.textfsm
--rw-r--r--   0        0        0      954 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm
--rw-r--r--   0        0        0      233 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_cts_interface_brief.textfsm
--rw-r--r--   0        0        0     2143 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm
--rw-r--r--   0        0        0      384 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_environment_temperature.textfsm
--rw-r--r--   0        0        0      147 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_feature.textfsm
--rw-r--r--   0        0        0      178 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_fex.textfsm
--rw-r--r--   0        0        0     1002 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm
--rw-r--r--   0        0        0      491 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_flogi_database.textfsm
--rw-r--r--   0        0        0     1083 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm
--rw-r--r--   0        0        0      979 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm
--rw-r--r--   0        0        0       57 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_hostname.textfsm
--rw-r--r--   0        0        0     2323 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm
--rw-r--r--   0        0        0     1491 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm
--rw-r--r--   0        0        0     1571 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm
--rw-r--r--   0        0        0      358 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface_description.textfsm
--rw-r--r--   0        0        0      364 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface_status.textfsm
--rw-r--r--   0        0        0      518 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm
--rw-r--r--   0        0        0     2240 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm
--rw-r--r--   0        0        0      800 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm
--rw-r--r--   0        0        0      500 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_inventory.textfsm
--rw-r--r--   0        0        0      698 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm
--rw-r--r--   0        0        0      300 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_arp.textfsm
--rw-r--r--   0        0        0      426 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_arp_detail.textfsm
--rw-r--r--   0        0        0     2011 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm
--rw-r--r--   0        0        0     4318 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm
--rw-r--r--   0        0        0      974 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0     1014 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm
--rw-r--r--   0        0        0      714 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm
--rw-r--r--   0        0        0      283 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_relay_address.textfsm
--rw-r--r--   0        0        0     3956 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm
--rw-r--r--   0        0        0     5936 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm
--rw-r--r--   0        0        0      356 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0     2403 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm
--rw-r--r--   0        0        0      680 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm
--rw-r--r--   0        0        0      526 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      387 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_neighbor.textfsm
--rw-r--r--   0        0        0     2072 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm
--rw-r--r--   0        0        0      222 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      244 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_l2rib_internal_permanently-frozen-list.textfsm
--rw-r--r--   0        0        0      411 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_license_usage.textfsm
--rw-r--r--   0        0        0      297 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      727 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      290 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      351 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_module.textfsm
--rw-r--r--   0        0        0      288 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_nve_peers.textfsm
--rw-r--r--   0        0        0      495 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_nve_vni.textfsm
--rw-r--r--   0        0        0     2346 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm
--rw-r--r--   0        0        0      234 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_processes_cpu.textfsm
--rw-r--r--   0        0        0      698 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm
--rw-r--r--   0        0        0      296 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_vdc.textfsm
--rwxr-xr-x   0        0        0      697 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_version.textfsm
--rw-r--r--   0        0        0     6310 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm
--rw-r--r--   0        0        0       99 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_vpc.textfsm
--rw-r--r--   0        0        0      279 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_vrf.textfsm
--rw-r--r--   0        0        0      239 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_vrf_interface.textfsm
--rw-r--r--   0        0        0      594 2023-03-21 20:38:25.452750 ntc_templates-3.3.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      411 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_s300_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      330 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_s300_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      442 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_s300_show_version.textfsm
--rw-r--r--   0        0        0     3155 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm
--rw-r--r--   0        0        0     4795 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm
--rw-r--r--   0        0        0     1683 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm
--rw-r--r--   0        0        0     2697 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm
--rw-r--r--   0        0        0      643 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm
--rw-r--r--   0        0        0      492 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_summary.textfsm
--rw-r--r--   0        0        0      780 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm
--rw-r--r--   0        0        0      661 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1429 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm
--rw-r--r--   0        0        0      276 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_exclusionlist.textfsm
--rw-r--r--   0        0        0      355 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_flexconnect_group_summary.textfsm
--rw-r--r--   0        0        0     1437 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm
--rw-r--r--   0        0        0      347 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_group_summary.textfsm
--rw-r--r--   0        0        0      480 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_summary.textfsm
--rw-r--r--   0        0        0      436 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_inventory.textfsm
--rw-r--r--   0        0        0      463 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_anchor.textfsm
--rw-r--r--   0        0        0      737 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm
--rw-r--r--   0        0        0      655 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm
--rw-r--r--   0        0        0     2799 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm
--rw-r--r--   0        0        0      842 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm
--rw-r--r--   0        0        0      970 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm
--rw-r--r--   0        0        0      417 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_rf-profile_summary.textfsm
--rw-r--r--   0        0        0      997 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm
--rw-r--r--   0        0        0     1238 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm
--rw-r--r--   0        0        0     1450 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm
--rw-r--r--   0        0        0      906 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm
--rw-r--r--   0        0        0      420 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_wlan_sum.textfsm
--rw-r--r--   0        0        0     6223 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm
--rw-r--r--   0        0        0     1379 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm
--rw-r--r--   0        0        0      309 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_admin_show_environment_power.textfsm
--rw-r--r--   0        0        0      461 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_admin_show_inventory.textfsm
--rw-r--r--   0        0        0      179 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_admin_show_platform.textfsm
--rw-r--r--   0        0        0      419 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_admin_show_vm.textfsm
--rw-r--r--   0        0        0      515 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_arp.textfsm
--rw-r--r--   0        0        0      838 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm
--rw-r--r--   0        0        0      179 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_bfd_sessions.textfsm
--rw-r--r--   0        0        0     1905 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm
--rw-r--r--   0        0        0      725 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm
--rw-r--r--   0        0        0     5397 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm
--rw-r--r--   0        0        0      156 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_bgp_vrf_all_ipv4_unicast_summary.textfsm
--rw-r--r--   0        0        0      513 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1544 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm
--rw-r--r--   0        0        0      337 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_configuration_commit_list.textfsm
--rw-r--r--   0        0        0      347 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controller_fabric_plane_all.textfsm
--rw-r--r--   0        0        0     2208 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm
--rw-r--r--   0        0        0     2281 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm
--rw-r--r--   0        0        0     2823 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm
--rw-r--r--   0        0        0     1961 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm
--rw-r--r--   0        0        0      426 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_egress_location.textfsm
--rw-r--r--   0        0        0     1406 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm
--rw-r--r--   0        0        0     4953 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm
--rw-r--r--   0        0        0      266 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_dhcp_ipv4_proxy_binding.textfsm
--rw-r--r--   0        0        0     7430 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm
--rw-r--r--   0        0        0      518 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm
--rw-r--r--   0        0        0      665 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm
--rw-r--r--   0        0        0      268 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_interface_brief.textfsm
--rw-r--r--   0        0        0      835 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm
--rw-r--r--   0        0        0      353 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_interfaces_summary.textfsm
--rw-r--r--   0        0        0      571 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0      178 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0     1094 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm
--rw-r--r--   0        0        0      769 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm
--rw-r--r--   0        0        0      270 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ipv4_vrf_all_interface_brief.textfsm
--rw-r--r--   0        0        0      405 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      288 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_isis_neighbors.textfsm
--rw-r--r--   0        0        0      380 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      694 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm
--rw-r--r--   0        0        0      398 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_mpls_ldp_neighbor_brief.textfsm
--rw-r--r--   0        0        0      356 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      440 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_interface_brief.textfsm
--rw-r--r--   0        0        0      474 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_neighbor.textfsm
--rw-r--r--   0        0        0      359 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_group-map.textfsm
--rw-r--r--   0        0        0      481 2023-03-21 20:38:25.456750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_interface.textfsm
--rw-r--r--   0        0        0      447 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_neighbor.textfsm
--rw-r--r--   0        0        0      262 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_pim_neighbor.textfsm
--rw-r--r--   0        0        0     1074 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm
--rw-r--r--   0        0        0      205 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_processes_cpu.textfsm
--rw-r--r--   0        0        0      187 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_redundancy_summary.textfsm
--rw-r--r--   0        0        0      226 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_rsvp_neighbors.textfsm
--rw-r--r--   0        0        0      856 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_version.textfsm
--rw-r--r--   0        0        0      339 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_version_brief.textfsm
--rw-r--r--   0        0        0      422 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_vrf_all_detail.textfsm
--rw-r--r--   0        0        0      290 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/dell_force10_show_arp.textfsm
--rw-r--r--   0        0        0      213 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/dell_force10_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      211 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/dell_force10_show_version.textfsm
--rw-r--r--   0        0        0      815 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/dell_force10_show_vlan.textfsm
--rw-r--r--   0        0        0      248 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/dell_force10_show_vlan_brief.textfsm
--rw-r--r--   0        0        0      289 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/dell_powerconnect_show_bridge_address_table.textfsm
--rw-r--r--   0        0        0      193 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/dell_powerconnect_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      592 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      301 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/dlink_ds_show_arpentry.textfsm
--rw-r--r--   0        0        0      647 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm
--rw-r--r--   0        0        0      433 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/ericsson_ipos_show_isis_adjacency.textfsm
--rw-r--r--   0        0        0      168 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/ericsson_ipos_show_version.textfsm
--rw-r--r--   0        0        0      574 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm
--rw-r--r--   0        0        0      230 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_system_arp.textfsm
--rw-r--r--   0        0        0     2048 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm
--rw-r--r--   0        0        0     8998 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_system_interface.textfsm
--rw-r--r--   0        0        0      657 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm
--rw-r--r--   0        0        0     2528 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_system_status.textfsm
--rw-r--r--   0        0        0      238 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_arp.textfsm
--rw-r--r--   0        0        0      200 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_clock.textfsm
--rw-r--r--   0        0        0      519 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm
--rw-r--r--   0        0        0      666 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm
--rw-r--r--   0        0        0     8289 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_interface.textfsm
--rw-r--r--   0        0        0     1478 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm
--rw-r--r--   0        0        0      616 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm
--rw-r--r--   0        0        0      195 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance.textfsm
--rw-r--r--   0        0        0     5480 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm
--rw-r--r--   0        0        0      777 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm
--rw-r--r--   0        0        0      397 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm
--rw-r--r--   0        0        0      926 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm
--rw-r--r--   0        0        0      187 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_mac-address.textfsm
--rw-r--r--   0        0        0      582 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm
--rw-r--r--   0        0        0      106 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_vlan_brief.textfsm
--rw-r--r--   0        0        0      179 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_arp.textfsm
--rw-r--r--   0        0        0      710 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm
--rw-r--r--   0        0        0      917 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      706 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm
--rw-r--r--   0        0        0     1699 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm
--rw-r--r--   0        0        0      222 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_mac-address.textfsm
--rw-r--r--   0        0        0      453 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_port-security.textfsm
--rw-r--r--   0        0        0     1329 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_system.textfsm
--rw-r--r--   0        0        0      385 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_tech_buffers.textfsm
--rw-r--r--   0        0        0      407 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_trunks.textfsm
--rw-r--r--   0        0        0      290 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_vlans.textfsm
--rw-r--r--   0        0        0     1133 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm
--rw-r--r--   0        0        0      551 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm
--rw-r--r--   0        0        0      491 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_arp_brief.textfsm
--rw-r--r--   0        0        0     3608 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm
--rw-r--r--   0        0        0      498 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_interface_brief.textfsm
--rw-r--r--   0        0        0      376 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_interface_description.textfsm
--rw-r--r--   0        0        0     2059 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm
--rw-r--r--   0        0        0      843 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      435 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_isis_peer.textfsm
--rw-r--r--   0        0        0     1811 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm
--rw-r--r--   0        0        0      713 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm
--rw-r--r--   0        0        0     7310 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm
--rw-r--r--   0        0        0      193 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_service-set_all.textfsm
--rw-r--r--   0        0        0     1084 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm
--rw-r--r--   0        0        0       96 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_sn_license.textfsm
--rw-r--r--   0        0        0      424 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_snmp-agent_community_read.textfsm
--rw-r--r--   0        0        0     1346 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm
--rw-r--r--   0        0        0      390 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_temperature.textfsm
--rw-r--r--   0        0        0      522 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm
--rw-r--r--   0        0        0      505 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_version.textfsm
--rw-r--r--   0        0        0    51752 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/index
--rw-r--r--   0        0        0      536 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm
--rw-r--r--   0        0        0      303 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_arp_no-resolve.textfsm
--rw-r--r--   0        0        0     3195 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm
--rw-r--r--   0        0        0      803 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm
--rw-r--r--   0        0        0      341 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_chassis_firmware.textfsm
--rw-r--r--   0        0        0      855 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm
--rw-r--r--   0        0        0      729 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm
--rw-r--r--   0        0        0      553 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm
--rw-r--r--   0        0        0      267 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_isis_adjacency.textfsm
--rw-r--r--   0        0        0      630 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm
--rw-r--r--   0        0        0      389 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      292 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_ospf_neighbor.textfsm
--rw-r--r--   0        0        0     1374 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm
--rw-r--r--   0        0        0     4359 2023-03-21 20:38:25.460750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_version.textfsm
--rw-r--r--   0        0        0      318 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_vlans.textfsm
--rw-r--r--   0        0        0      768 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/juniper_screenos_get_route.textfsm
--rw-r--r--   0        0        0      338 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/linux_arp_-a.textfsm
--rw-r--r--   0        0        0      915 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/linux_ip_address_show.textfsm
--rw-r--r--   0        0        0     1092 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/linux_ip_link_show.textfsm
--rw-r--r--   0        0        0      618 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/linux_ip_route_show.textfsm
--rw-r--r--   0        0        0      134 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/linux_ip_vrf_show.textfsm
--rw-r--r--   0        0        0      660 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm
--rw-r--r--   0        0        0      364 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ip_arp_print_without-paging.textfsm
--rw-r--r--   0        0        0      899 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm
--rw-r--r--   0        0        0     2499 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm
--rw-r--r--   0        0        0     2229 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm
--rw-r--r--   0        0        0      546 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm
--rw-r--r--   0        0        0      400 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ipv6_neighbor_print_without-paging.textfsm
--rw-r--r--   0        0        0      483 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_snmp_community_print_without-paging.textfsm
--rw-r--r--   0        0        0      673 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm
--rw-r--r--   0        0        0      169 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_debug_swm_status.textfsm
--rw-r--r--   0        0        0      337 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_arp_all.textfsm
--rw-r--r--   0        0        0      249 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_counter_global.textfsm
--rw-r--r--   0        0        0     1943 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm
--rw-r--r--   0        0        0      293 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_interface_hardware.textfsm
--rw-r--r--   0        0        0      256 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_interface_logical.textfsm
--rw-r--r--   0        0        0      962 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm
--rw-r--r--   0        0        0      415 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_jobs_all.textfsm
--rw-r--r--   0        0        0      236 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_mac_all.textfsm
--rw-r--r--   0        0        0      729 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm
--rw-r--r--   0        0        0      794 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm
--rw-r--r--   0        0        0      840 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm
--rw-r--r--   0        0        0      975 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm
--rw-r--r--   0        0        0      908 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm
--rw-r--r--   0        0        0      693 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm
--rw-r--r--   0        0        0      602 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      279 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_mac-address.textfsm
--rw-r--r--   0        0        0      263 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_media_validation.textfsm
--rw-r--r--   0        0        0     1049 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm
--rw-r--r--   0        0        0     2669 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm
--rw-r--r--   0        0        0      378 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_arp.textfsm
--rw-r--r--   0        0        0      372 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcp_leases.textfsm
--rw-r--r--   0        0        0      270 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcpv6_server_leases.textfsm
--rw-r--r--   0        0        0      293 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces.textfsm
--rw-r--r--   0        0        0      307 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces_ethernet_physical.textfsm
--rw-r--r--   0        0        0      662 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm
--rw-r--r--   0        0        0      224 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      471 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_route.textfsm
--rw-r--r--   0        0        0      380 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_version.textfsm
--rw-r--r--   0        0        0      314 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgeswitch_show_arp.textfsm
--rw-r--r--   0        0        0      553 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm
--rw-r--r--   0        0        0      209 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgeswitch_show_vlan.textfsm
--rw-r--r--   0        0        0      470 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/vmware_nsxv_show_ip_bgp_neighbors.textfsm
--rw-r--r--   0        0        0      259 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/vmware_nsxv_show_ip_route.textfsm
--rw-r--r--   0        0        0      281 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/vyatta_vyos_show_arp.textfsm
--rw-r--r--   0        0        0      374 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/vyatta_vyos_show_interfaces.textfsm
--rw-r--r--   0        0        0      859 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0      231 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/watchguard_firebox_show_arp.textfsm
--rw-r--r--   0        0        0     1181 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/yamaha_show_environment.textfsm
--rw-r--r--   0        0        0      472 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/yamaha_show_ip_route.textfsm
--rw-r--r--   0        0        0      626 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm
--rw-r--r--   0        0        0      402 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_intf_group_get.textfsm
--rw-r--r--   0        0        0      563 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm
--rw-r--r--   0        0        0      409 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_lan_get.textfsm
--rw-r--r--   0        0        0      662 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm
--rw-r--r--   0        0        0      411 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_lanhosts_get.textfsm
--rw-r--r--   0        0        0      664 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm
--rw-r--r--   0        0        0      751 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm
--rw-r--r--   0        0        0      629 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm
--rw-r--r--   0        0        0      339 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_static_dhcp_get.textfsm
--rw-r--r--   0        0        0      625 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm
--rw-r--r--   0        0        0      539 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm
--rw-r--r--   0        0        0      857 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm
--rw-r--r--   0        0        0      337 2023-03-21 20:38:25.464750 ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_zycli_Ethctl_media-type.textfsm
--rw-r--r--   0        0        0     3098 2023-03-21 20:38:39.444798 ntc_templates-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 ntc_templates-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0      601 2023-06-11 21:19:30.876631 ntc_templates-3.4.0/LICENSE
+-rw-r--r--   0        0        0     2842 2023-06-11 21:19:30.876631 ntc_templates-3.4.0/README.md
+-rw-r--r--   0        0        0      260 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/__init__.py
+-rw-r--r--   0        0        0     2180 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/parse.py
+-rw-r--r--   0        0        0      700 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm
+-rw-r--r--   0        0        0      170 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_oam_mac-ping.textfsm
+-rw-r--r--   0        0        0      371 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_lag.textfsm
+-rw-r--r--   0        0        0      641 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_port.textfsm
+-rw-r--r--   0        0        0      434 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_bgp_routes_vpn-ipv4.textfsm
+-rw-r--r--   0        0        0      526 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm
+-rw-r--r--   0        0        0      662 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm
+-rw-r--r--   0        0        0      318 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_isis_adjacency.textfsm
+-rw-r--r--   0        0        0      336 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_isis_interface.textfsm
+-rw-r--r--   0        0        0      619 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm
+-rw-r--r--   0        0        0      608 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm
+-rw-r--r--   0        0        0      512 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm
+-rw-r--r--   0        0        0      547 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm
+-rw-r--r--   0        0        0      425 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_pim_interface.textfsm
+-rw-r--r--   0        0        0      649 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm
+-rw-r--r--   0        0        0      544 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm
+-rw-r--r--   0        0        0      665 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm
+-rw-r--r--   0        0        0      598 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm
+-rw-r--r--   0        0        0      642 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm
+-rw-r--r--   0        0        0      522 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm
+-rw-r--r--   0        0        0      371 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_bash_df_-h.textfsm
+-rw-r--r--   0        0        0      430 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_dir_flash.textfsm
+-rw-r--r--   0        0        0      121 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_boot-config.textfsm
+-rw-r--r--   0        0        0      226 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_clock.textfsm
+-rw-r--r--   0        0        0      524 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm
+-rw-r--r--   0        0        0      525 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm
+-rw-r--r--   0        0        0      107 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_hostname.textfsm
+-rw-r--r--   0        0        0      888 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm
+-rw-r--r--   0        0        0      427 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      399 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      313 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver.textfsm
+-rw-r--r--   0        0        0      757 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm
+-rw-r--r--   0        0        0      666 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_inventory.textfsm
+-rw-r--r--   0        0        0      517 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm
+-rw-r--r--   0        0        0      159 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_arp.textfsm
+-rw-r--r--   0        0        0      651 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm
+-rw-r--r--   0        0        0     1568 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0      246 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_helper-address.textfsm
+-rw-r--r--   0        0        0      169 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      736 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm
+-rw-r--r--   0        0        0      387 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      462 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      734 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm
+-rw-r--r--   0        0        0     1035 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm
+-rw-r--r--   0        0        0     1101 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm
+-rw-r--r--   0        0        0      358 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_isis_neighbors.textfsm
+-rw-r--r--   0        0        0      190 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      627 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1662 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      257 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_security_interface.textfsm
+-rw-r--r--   0        0        0      303 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_security_mka_counters.textfsm
+-rw-r--r--   0        0        0     1431 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm
+-rw-r--r--   0        0        0      279 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mlag.textfsm
+-rw-r--r--   0        0        0      716 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_module.textfsm
+-rw-r--r--   0        0        0      557 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm
+-rw-r--r--   0        0        0      403 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_pim_ipv4_neighbor.textfsm
+-rw-r--r--   0        0        0     1222 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm
+-rw-r--r--   0        0        0     5405 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm
+-rw-r--r--   0        0        0      573 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm
+-rw-r--r--   0        0        0      275 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_snmp_community.textfsm
+-rw-r--r--   0        0        0      424 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_version.textfsm
+-rw-r--r--   0        0        0     6187 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_vlan.textfsm
+-rw-r--r--   0        0        0     4153 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_vrf.textfsm
+-rw-r--r--   0        0        0      701 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm
+-rw-r--r--   0        0        0      322 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_arp_all-vrfs.textfsm
+-rw-r--r--   0        0        0      596 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm
+-rw-r--r--   0        0        0      531 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm
+-rw-r--r--   0        0        0      531 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm
+-rw-r--r--   0        0        0     2201 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm
+-rw-r--r--   0        0        0     4761 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm
+-rw-r--r--   0        0        0      348 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_ip_route_all-vrfs.textfsm
+-rw-r--r--   0        0        0      827 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm
+-rw-r--r--   0        0        0      240 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0      380 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_ntp_associations.textfsm
+-rw-r--r--   0        0        0      662 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm
+-rw-r--r--   0        0        0      917 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm
+-rw-r--r--   0        0        0      768 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm
+-rw-r--r--   0        0        0     1028 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm
+-rw-r--r--   0        0        0      977 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm
+-rw-r--r--   0        0        0      735 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_arp.textfsm
+-rw-r--r--   0        0        0      176 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      287 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      119 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_interface_name.textfsm
+-rw-r--r--   0        0        0      702 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm
+-rw-r--r--   0        0        0      181 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0      878 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm
+-rw-r--r--   0        0        0      607 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm
+-rw-r--r--   0        0        0     1825 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm
+-rw-r--r--   0        0        0      470 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_vlan.textfsm
+-rw-r--r--   0        0        0      367 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_vsp_show_software.textfsm
+-rw-r--r--   0        0        0      583 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm
+-rw-r--r--   0        0        0      631 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm
+-rw-r--r--   0        0        0      458 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_mac-addr-table.textfsm
+-rw-r--r--   0        0        0     1497 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_version.textfsm
+-rw-r--r--   0        0        0      372 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_vlan_brief.textfsm
+-rw-r--r--   0        0        0      358 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_arp.textfsm
+-rw-r--r--   0        0        0     5683 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm
+-rw-r--r--   0        0        0      695 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      367 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_lag_brief.textfsm
+-rw-r--r--   0        0        0      416 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      906 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      375 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_mac-address.textfsm
+-rw-r--r--   0        0        0     1120 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm
+-rw-r--r--   0        0        0      301 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_monitor.textfsm
+-rw-r--r--   0        0        0     2278 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm
+-rw-r--r--   0        0        0      851 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm
+-rw-r--r--   0        0        0      351 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_topo.textfsm
+-rw-r--r--   0        0        0     2990 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm
+-rw-r--r--   0        0        0     1629 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm
+-rw-r--r--   0        0        0     6614 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm
+-rw-r--r--   0        0        0      430 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      367 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_lag_brief.textfsm
+-rw-r--r--   0        0        0      906 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1071 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm
+-rw-r--r--   0        0        0      311 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_monitor_actual.textfsm
+-rw-r--r--   0        0        0     1618 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm
+-rw-r--r--   0        0        0     2277 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm
+-rw-r--r--   0        0        0      739 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_span.textfsm
+-rw-r--r--   0        0        0      591 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm
+-rw-r--r--   0        0        0      167 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_fw_stat.textfsm
+-rw-r--r--   0        0        0      170 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_arp_dynamic_all.textfsm
+-rw-r--r--   0        0        0      148 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_asset_all.textfsm
+-rw-r--r--   0        0        0      189 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_dns.textfsm
+-rw-r--r--   0        0        0       71 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_domainname.textfsm
+-rw-r--r--   0        0        0      786 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm
+-rw-r--r--   0        0        0      482 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      159 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_lom.textfsm
+-rw-r--r--   0        0        0      208 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_ntp_servers.textfsm
+-rw-r--r--   0        0        0      550 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm
+-rw-r--r--   0        0        0      236 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_version_all.textfsm
+-rw-r--r--   0        0        0      419 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_chassis_show_temperature.textfsm
+-rw-r--r--   0        0        0     1010 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_port_show.textfsm
+-rw-r--r--   0        0        0      945 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm
+-rw-r--r--   0        0        0      623 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_software_show.textfsm
+-rw-r--r--   0        0        0      289 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_ssh_server_show_key.textfsm
+-rw-r--r--   0        0        0      556 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm
+-rw-r--r--   0        0        0      636 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm
+-rw-r--r--   0        0        0      714 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm
+-rw-r--r--   0        0        0      663 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_dir.textfsm
+-rw-r--r--   0        0        0      661 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_ping.textfsm
+-rw-r--r--   0        0        0     4925 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm
+-rw-r--r--   0        0        0      325 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_arp.textfsm
+-rw-r--r--   0        0        0     9761 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm
+-rw-r--r--   0        0        0      829 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm
+-rw-r--r--   0        0        0     1377 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm
+-rw-r--r--   0        0        0      917 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm
+-rw-r--r--   0        0        0      438 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_crypto_ikev1_sa_detail.textfsm
+-rw-r--r--   0        0        0     6136 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm
+-rw-r--r--   0        0        0     3036 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_failover.textfsm
+-rw-r--r--   0        0        0     4402 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface.textfsm
+-rw-r--r--   0        0        0     7080 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm
+-rw-r--r--   0        0        0      268 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface_ip_brief.textfsm
+-rw-r--r--   0        0        0      320 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_inventory.textfsm
+-rw-r--r--   0        0        0     4240 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm
+-rw-r--r--   0        0        0     2352 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_logging.textfsm
+-rw-r--r--   0        0        0       89 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_name.textfsm
+-rw-r--r--   0        0        0     1624 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_nat.textfsm
+-rw-r--r--   0        0        0      561 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm
+-rw-r--r--   0        0        0      403 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      374 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0     1208 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm
+-rw-r--r--   0        0        0      425 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_resource_usage.textfsm
+-rw-r--r--   0        0        0     1606 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_route.textfsm
+-rw-r--r--   0        0        0     2300 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm
+-rw-r--r--   0        0        0      437 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_ikev1.textfsm
+-rw-r--r--   0        0        0     1212 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm
+-rw-r--r--   0        0        0     1726 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm
+-rw-r--r--   0        0        0      474 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_object_network.textfsm
+-rw-r--r--   0        0        0     4906 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm
+-rw-r--r--   0        0        0      967 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_version.textfsm
+-rw-r--r--   0        0        0     1625 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm
+-rw-r--r--   0        0        0     1822 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm
+-rw-r--r--   0        0        0     7479 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm
+-rw-r--r--   0        0        0     1126 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm
+-rw-r--r--   0        0        0      481 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_dir.textfsm
+-rw-r--r--   0        0        0      859 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_ping.textfsm
+-rw-r--r--   0        0        0     1584 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm
+-rw-r--r--   0        0        0      416 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_access-session.textfsm
+-rw-r--r--   0        0        0      953 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm
+-rw-r--r--   0        0        0      355 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_alert_counters.textfsm
+-rw-r--r--   0        0        0      310 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_aliases.textfsm
+-rw-r--r--   0        0        0      523 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm
+-rw-r--r--   0        0        0      615 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_archive.textfsm
+-rw-r--r--   0        0        0      403 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_authentication_sessions.textfsm
+-rw-r--r--   0        0        0     2496 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm
+-rw-r--r--   0        0        0     1700 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_boot.textfsm
+-rw-r--r--   0        0        0      264 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_capability_feature_routing.textfsm
+-rw-r--r--   0        0        0      538 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm
+-rw-r--r--   0        0        0      937 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      317 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_clock.textfsm
+-rw-r--r--   0        0        0     2327 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm
+-rw-r--r--   0        0        0     6120 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm
+-rw-r--r--   0        0        0     2174 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm
+-rw-r--r--   0        0        0     1418 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm
+-rw-r--r--   0        0        0     1041 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm
+-rw-r--r--   0        0        0      491 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dmvpn.textfsm
+-rw-r--r--   0        0        0     1367 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm
+-rw-r--r--   0        0        0      413 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_environment_power_all.textfsm
+-rw-r--r--   0        0        0     1603 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm
+-rw-r--r--   0        0        0     1188 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm
+-rw-r--r--   0        0        0      454 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_hosts_summary.textfsm
+-rw-r--r--   0        0        0     1226 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm
+-rw-r--r--   0        0        0      312 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interface_transceiver.textfsm
+-rw-r--r--   0        0        0     2729 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm
+-rw-r--r--   0        0        0      409 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      898 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0     1512 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm
+-rw-r--r--   0        0        0      570 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm
+-rw-r--r--   0        0        0     2587 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm
+-rw-r--r--   0        0        0      525 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm
+-rw-r--r--   0        0        0     2029 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm
+-rw-r--r--   0        0        0     1706 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0     2011 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm
+-rw-r--r--   0        0        0      589 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0     1761 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm
+-rw-r--r--   0        0        0     1207 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm
+-rw-r--r--   0        0        0     3244 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm
+-rw-r--r--   0        0        0      711 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm
+-rw-r--r--   0        0        0     2669 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm
+-rw-r--r--   0        0        0      773 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm
+-rw-r--r--   0        0        0     2597 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm
+-rwxr-xr-x   0        0        0      459 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_flow_toptalkers.textfsm
+-rw-r--r--   0        0        0     4260 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm
+-rw-r--r--   0        0        0     1909 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm
+-rw-r--r--   0        0        0      288 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0     1378 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm
+-rw-r--r--   0        0        0      645 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm
+-rw-r--r--   0        0        0      778 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm
+-rw-r--r--   0        0        0     1362 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm
+-rw-r--r--   0        0        0     1807 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm
+-rw-r--r--   0        0        0      396 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      383 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      436 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_prefix-list.textfsm
+-rw-r--r--   0        0        0     2499 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm
+-rw-r--r--   0        0        0     1389 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm
+-rw-r--r--   0        0        0      555 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm
+-rw-r--r--   0        0        0      472 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_vrf_interfaces.textfsm
+-rw-r--r--   0        0        0      917 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm
+-rw-r--r--   0        0        0      399 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      371 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      523 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      956 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm
+-rw-r--r--   0        0        0      412 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_isis_neighbors.textfsm
+-rw-r--r--   0        0        0      547 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_license.textfsm
+-rw-r--r--   0        0        0      479 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0     2655 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     5593 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_logging.textfsm
+-rw-r--r--   0        0        0     4086 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0     1017 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module.textfsm
+-rw-r--r--   0        0        0      585 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm
+-rw-r--r--   0        0        0     1062 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm
+-rw-r--r--   0        0        0      760 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm
+-rw-r--r--   0        0        0      350 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_mpls_interfaces.textfsm
+-rw-r--r--   0        0        0      377 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_nve_peers.textfsm
+-rw-r--r--   0        0        0      346 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_nve_vni.textfsm
+-rw-r--r--   0        0        0     1215 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm
+-rw-r--r--   0        0        0     1072 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm
+-rw-r--r--   0        0        0      974 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm
+-rw-r--r--   0        0        0      922 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm
+-rw-r--r--   0        0        0      684 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm
+-rw-r--r--   0        0        0      314 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_supplies.textfsm
+-rw-r--r--   0        0        0      344 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_processes_cpu.textfsm
+-rw-r--r--   0        0        0      640 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm
+-rw-r--r--   0        0        0     3950 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm
+-rw-r--r--   0        0        0      784 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm
+-rw-r--r--   0        0        0     3318 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm
+-rw-r--r--   0        0        0     1034 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm
+-rw-r--r--   0        0        0      359 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_community.textfsm
+-rw-r--r--   0        0        0      802 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm
+-rw-r--r--   0        0        0      668 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm
+-rw-r--r--   0        0        0      413 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_spanning-tree.textfsm
+-rw-r--r--   0        0        0     2018 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_standby.textfsm
+-rw-r--r--   0        0        0      621 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm
+-rw-r--r--   0        0        0      495 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_switch_detail.textfsm
+-rw-r--r--   0        0        0      357 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_switch_detail_stack_ports.textfsm
+-rw-r--r--   0        0        0     1009 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm
+-rw-r--r--   0        0        0     1735 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_version.textfsm
+-rw-r--r--   0        0        0     6327 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm
+-rw-r--r--   0        0        0      534 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm
+-rw-r--r--   0        0        0     1047 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrf_detail.textfsm
+-rw-r--r--   0        0        0     1596 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm
+-rw-r--r--   0        0        0     1655 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm
+-rw-r--r--   0        0        0     1109 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm
+-rw-r--r--   0        0        0     1660 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_traceroute.textfsm
+-rw-r--r--   0        0        0     1781 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm
+-rw-r--r--   0        0        0      461 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors.textfsm
+-rw-r--r--   0        0        0      689 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      203 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_clock.textfsm
+-rw-r--r--   0        0        0      210 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_configuration_session_summary.textfsm
+-rw-r--r--   0        0        0      954 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm
+-rw-r--r--   0        0        0      233 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cts_interface_brief.textfsm
+-rw-r--r--   0        0        0     2143 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm
+-rw-r--r--   0        0        0      384 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_environment_temperature.textfsm
+-rw-r--r--   0        0        0      147 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_feature.textfsm
+-rw-r--r--   0        0        0      178 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_fex.textfsm
+-rw-r--r--   0        0        0     1002 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm
+-rw-r--r--   0        0        0      491 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_flogi_database.textfsm
+-rw-r--r--   0        0        0     1083 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm
+-rw-r--r--   0        0        0      979 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm
+-rw-r--r--   0        0        0       57 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_hostname.textfsm
+-rw-r--r--   0        0        0     2323 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm
+-rw-r--r--   0        0        0     1491 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm
+-rw-r--r--   0        0        0     1717 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm
+-rw-r--r--   0        0        0      358 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_description.textfsm
+-rw-r--r--   0        0        0      364 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_status.textfsm
+-rw-r--r--   0        0        0      518 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm
+-rw-r--r--   0        0        0     2240 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm
+-rw-r--r--   0        0        0      800 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm
+-rw-r--r--   0        0        0      500 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_inventory.textfsm
+-rw-r--r--   0        0        0      698 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm
+-rw-r--r--   0        0        0      300 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_arp.textfsm
+-rw-r--r--   0        0        0      426 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_arp_detail.textfsm
+-rw-r--r--   0        0        0     2011 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm
+-rw-r--r--   0        0        0     4318 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0      974 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0     1014 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm
+-rw-r--r--   0        0        0      714 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm
+-rw-r--r--   0        0        0      283 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_relay_address.textfsm
+-rw-r--r--   0        0        0     3956 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm
+-rw-r--r--   0        0        0     5936 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm
+-rw-r--r--   0        0        0      356 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0     2403 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm
+-rw-r--r--   0        0        0      665 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm
+-rw-r--r--   0        0        0      680 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm
+-rw-r--r--   0        0        0      526 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      387 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      453 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_group-range_vrf_all.textfsm
+-rw-r--r--   0        0        0      480 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_interface_brief_vrf_all.textfsm
+-rw-r--r--   0        0        0      599 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm
+-rw-r--r--   0        0        0      546 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_rp_vrf_all.textfsm
+-rw-r--r--   0        0        0     2072 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm
+-rw-r--r--   0        0        0      222 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      244 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_l2rib_internal_permanently-frozen-list.textfsm
+-rw-r--r--   0        0        0      411 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_license_usage.textfsm
+-rw-r--r--   0        0        0      297 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      727 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      290 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      351 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_module.textfsm
+-rw-r--r--   0        0        0      288 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_nve_peers.textfsm
+-rw-r--r--   0        0        0      495 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_nve_vni.textfsm
+-rw-r--r--   0        0        0     2346 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm
+-rw-r--r--   0        0        0      234 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_processes_cpu.textfsm
+-rw-r--r--   0        0        0      698 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm
+-rw-r--r--   0        0        0      489 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_spanning-tree_root.textfsm
+-rw-r--r--   0        0        0      296 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vdc.textfsm
+-rwxr-xr-x   0        0        0      697 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_version.textfsm
+-rw-r--r--   0        0        0     6310 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm
+-rw-r--r--   0        0        0       99 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vpc.textfsm
+-rw-r--r--   0        0        0      279 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vrf.textfsm
+-rw-r--r--   0        0        0      239 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vrf_interface.textfsm
+-rw-r--r--   0        0        0      594 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      411 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      330 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      442 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_version.textfsm
+-rw-r--r--   0        0        0     3155 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm
+-rw-r--r--   0        0        0     4795 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm
+-rw-r--r--   0        0        0     1683 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm
+-rw-r--r--   0        0        0     2697 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm
+-rw-r--r--   0        0        0      643 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm
+-rw-r--r--   0        0        0      492 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_summary.textfsm
+-rw-r--r--   0        0        0      780 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm
+-rw-r--r--   0        0        0      661 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1429 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm
+-rw-r--r--   0        0        0      276 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_exclusionlist.textfsm
+-rw-r--r--   0        0        0      355 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_flexconnect_group_summary.textfsm
+-rw-r--r--   0        0        0     1437 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm
+-rw-r--r--   0        0        0      347 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_group_summary.textfsm
+-rw-r--r--   0        0        0      480 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_summary.textfsm
+-rw-r--r--   0        0        0      436 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_inventory.textfsm
+-rw-r--r--   0        0        0      463 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_anchor.textfsm
+-rw-r--r--   0        0        0      737 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm
+-rw-r--r--   0        0        0      655 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm
+-rw-r--r--   0        0        0     2799 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm
+-rw-r--r--   0        0        0      842 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm
+-rw-r--r--   0        0        0      970 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm
+-rw-r--r--   0        0        0      417 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_rf-profile_summary.textfsm
+-rw-r--r--   0        0        0      997 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm
+-rw-r--r--   0        0        0     1238 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm
+-rw-r--r--   0        0        0     1450 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm
+-rw-r--r--   0        0        0      906 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm
+-rw-r--r--   0        0        0      420 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_wlan_sum.textfsm
+-rw-r--r--   0        0        0     6223 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm
+-rw-r--r--   0        0        0     1379 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm
+-rw-r--r--   0        0        0      309 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_environment_power.textfsm
+-rw-r--r--   0        0        0      398 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_inventory.textfsm
+-rw-r--r--   0        0        0      179 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_platform.textfsm
+-rw-r--r--   0        0        0      419 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_vm.textfsm
+-rw-r--r--   0        0        0      515 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_arp.textfsm
+-rw-r--r--   0        0        0      838 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm
+-rw-r--r--   0        0        0      179 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bfd_sessions.textfsm
+-rw-r--r--   0        0        0     1905 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm
+-rw-r--r--   0        0        0      725 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm
+-rw-r--r--   0        0        0     5397 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0      156 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_vrf_all_ipv4_unicast_summary.textfsm
+-rw-r--r--   0        0        0      513 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1544 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm
+-rw-r--r--   0        0        0      337 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_configuration_commit_list.textfsm
+-rw-r--r--   0        0        0      347 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controller_fabric_plane_all.textfsm
+-rw-r--r--   0        0        0     2208 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm
+-rw-r--r--   0        0        0     2281 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm
+-rw-r--r--   0        0        0     2823 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm
+-rw-r--r--   0        0        0     1961 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm
+-rw-r--r--   0        0        0      426 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_egress_location.textfsm
+-rw-r--r--   0        0        0     1406 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm
+-rw-r--r--   0        0        0     4953 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm
+-rw-r--r--   0        0        0      266 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_dhcp_ipv4_proxy_binding.textfsm
+-rw-r--r--   0        0        0     7430 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm
+-rw-r--r--   0        0        0      518 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm
+-rw-r--r--   0        0        0      665 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm
+-rw-r--r--   0        0        0      268 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_interface_brief.textfsm
+-rw-r--r--   0        0        0      835 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm
+-rw-r--r--   0        0        0      353 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_interfaces_summary.textfsm
+-rw-r--r--   0        0        0      571 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0      178 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0     1094 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm
+-rw-r--r--   0        0        0      769 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm
+-rw-r--r--   0        0        0      270 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ipv4_vrf_all_interface_brief.textfsm
+-rw-r--r--   0        0        0      405 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      288 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_isis_neighbors.textfsm
+-rw-r--r--   0        0        0      380 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      694 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm
+-rw-r--r--   0        0        0      398 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_mpls_ldp_neighbor_brief.textfsm
+-rw-r--r--   0        0        0      356 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      440 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_interface_brief.textfsm
+-rw-r--r--   0        0        0      474 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_neighbor.textfsm
+-rw-r--r--   0        0        0      359 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_group-map.textfsm
+-rw-r--r--   0        0        0      481 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_interface.textfsm
+-rw-r--r--   0        0        0      447 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_neighbor.textfsm
+-rw-r--r--   0        0        0      262 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_pim_neighbor.textfsm
+-rw-r--r--   0        0        0     1074 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm
+-rw-r--r--   0        0        0      205 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_processes_cpu.textfsm
+-rw-r--r--   0        0        0      187 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_redundancy_summary.textfsm
+-rw-r--r--   0        0        0      226 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_rsvp_neighbors.textfsm
+-rw-r--r--   0        0        0      856 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_version.textfsm
+-rw-r--r--   0        0        0      339 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_version_brief.textfsm
+-rw-r--r--   0        0        0      422 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_vrf_all_detail.textfsm
+-rw-r--r--   0        0        0      290 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_arp.textfsm
+-rw-r--r--   0        0        0      213 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      211 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_version.textfsm
+-rw-r--r--   0        0        0      815 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_vlan.textfsm
+-rw-r--r--   0        0        0      248 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_vlan_brief.textfsm
+-rw-r--r--   0        0        0      289 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_powerconnect_show_bridge_address_table.textfsm
+-rw-r--r--   0        0        0      193 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_powerconnect_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      592 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      301 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dlink_ds_show_arpentry.textfsm
+-rw-r--r--   0        0        0      647 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm
+-rw-r--r--   0        0        0      433 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/ericsson_ipos_show_isis_adjacency.textfsm
+-rw-r--r--   0        0        0      168 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/ericsson_ipos_show_version.textfsm
+-rw-r--r--   0        0        0      574 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm
+-rw-r--r--   0        0        0      230 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_arp.textfsm
+-rw-r--r--   0        0        0     2048 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm
+-rw-r--r--   0        0        0     8998 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_interface.textfsm
+-rw-r--r--   0        0        0      657 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm
+-rw-r--r--   0        0        0     2528 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_status.textfsm
+-rw-r--r--   0        0        0      238 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_arp.textfsm
+-rw-r--r--   0        0        0      200 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_clock.textfsm
+-rw-r--r--   0        0        0      519 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm
+-rw-r--r--   0        0        0      666 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm
+-rw-r--r--   0        0        0     8519 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_interface.textfsm
+-rw-r--r--   0        0        0     1573 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm
+-rw-r--r--   0        0        0      616 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm
+-rw-r--r--   0        0        0      195 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance.textfsm
+-rw-r--r--   0        0        0     5480 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm
+-rw-r--r--   0        0        0      777 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm
+-rw-r--r--   0        0        0      647 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm
+-rw-r--r--   0        0        0      926 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm
+-rw-r--r--   0        0        0      187 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_mac-address.textfsm
+-rw-r--r--   0        0        0      632 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm
+-rw-r--r--   0        0        0      106 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_vlan_brief.textfsm
+-rw-r--r--   0        0        0      179 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_arp.textfsm
+-rw-r--r--   0        0        0      710 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm
+-rw-r--r--   0        0        0      917 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      706 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm
+-rw-r--r--   0        0        0     1699 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm
+-rw-r--r--   0        0        0      222 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_mac-address.textfsm
+-rw-r--r--   0        0        0      453 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_port-security.textfsm
+-rw-r--r--   0        0        0     1329 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_system.textfsm
+-rw-r--r--   0        0        0      385 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_tech_buffers.textfsm
+-rw-r--r--   0        0        0      407 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_trunks.textfsm
+-rw-r--r--   0        0        0      290 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_vlans.textfsm
+-rw-r--r--   0        0        0     1392 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm
+-rw-r--r--   0        0        0      551 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm
+-rw-r--r--   0        0        0      491 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_arp_brief.textfsm
+-rw-r--r--   0        0        0     3608 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm
+-rw-r--r--   0        0        0      498 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_interface_brief.textfsm
+-rw-r--r--   0        0        0      376 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_interface_description.textfsm
+-rw-r--r--   0        0        0     2059 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm
+-rw-r--r--   0        0        0      843 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      435 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_isis_peer.textfsm
+-rw-r--r--   0        0        0     1811 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm
+-rw-r--r--   0        0        0      713 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm
+-rw-r--r--   0        0        0     7310 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm
+-rw-r--r--   0        0        0      193 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_service-set_all.textfsm
+-rw-r--r--   0        0        0     1084 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm
+-rw-r--r--   0        0        0       96 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_sn_license.textfsm
+-rw-r--r--   0        0        0      424 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_snmp-agent_community_read.textfsm
+-rw-r--r--   0        0        0     1346 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm
+-rw-r--r--   0        0        0      390 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_temperature.textfsm
+-rw-r--r--   0        0        0      522 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm
+-rw-r--r--   0        0        0      505 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_version.textfsm
+-rw-r--r--   0        0        0    52562 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/index
+-rw-r--r--   0        0        0      536 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm
+-rw-r--r--   0        0        0      303 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_arp_no-resolve.textfsm
+-rw-r--r--   0        0        0     3195 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm
+-rw-r--r--   0        0        0      803 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm
+-rw-r--r--   0        0        0      341 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_firmware.textfsm
+-rw-r--r--   0        0        0      855 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm
+-rw-r--r--   0        0        0      729 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm
+-rw-r--r--   0        0        0      553 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm
+-rw-r--r--   0        0        0      267 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_isis_adjacency.textfsm
+-rw-r--r--   0        0        0      630 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm
+-rw-r--r--   0        0        0      389 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      292 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0     1374 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm
+-rw-r--r--   0        0        0     4359 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_version.textfsm
+-rw-r--r--   0        0        0      318 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_vlans.textfsm
+-rw-r--r--   0        0        0      768 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_screenos_get_route.textfsm
+-rw-r--r--   0        0        0      338 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_arp_-a.textfsm
+-rw-r--r--   0        0        0      915 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_ip_address_show.textfsm
+-rw-r--r--   0        0        0     1092 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_ip_link_show.textfsm
+-rw-r--r--   0        0        0      618 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_ip_route_show.textfsm
+-rw-r--r--   0        0        0      134 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_ip_vrf_show.textfsm
+-rw-r--r--   0        0        0      660 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm
+-rw-r--r--   0        0        0      364 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_arp_print_without-paging.textfsm
+-rw-r--r--   0        0        0      899 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm
+-rw-r--r--   0        0        0      331 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_address-list_print_terse.textfsm
+-rw-r--r--   0        0        0     2499 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm
+-rw-r--r--   0        0        0     2229 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm
+-rw-r--r--   0        0        0      546 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm
+-rw-r--r--   0        0        0      400 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ipv6_neighbor_print_without-paging.textfsm
+-rw-r--r--   0        0        0      483 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_snmp_community_print_without-paging.textfsm
+-rw-r--r--   0        0        0      673 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm
+-rw-r--r--   0        0        0      169 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_debug_swm_status.textfsm
+-rw-r--r--   0        0        0      337 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_arp_all.textfsm
+-rw-r--r--   0        0        0      249 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_counter_global.textfsm
+-rw-r--r--   0        0        0     1943 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm
+-rw-r--r--   0        0        0      293 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_interface_hardware.textfsm
+-rw-r--r--   0        0        0      256 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_interface_logical.textfsm
+-rw-r--r--   0        0        0      962 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm
+-rw-r--r--   0        0        0      415 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_jobs_all.textfsm
+-rw-r--r--   0        0        0      236 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_mac_all.textfsm
+-rw-r--r--   0        0        0      729 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm
+-rw-r--r--   0        0        0      794 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm
+-rw-r--r--   0        0        0      840 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm
+-rw-r--r--   0        0        0      975 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm
+-rw-r--r--   0        0        0      908 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm
+-rw-r--r--   0        0        0      693 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm
+-rw-r--r--   0        0        0      602 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      279 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_mac-address.textfsm
+-rw-r--r--   0        0        0      263 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_media_validation.textfsm
+-rw-r--r--   0        0        0     1049 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm
+-rw-r--r--   0        0        0     2669 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm
+-rw-r--r--   0        0        0      401 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_arp.textfsm
+-rw-r--r--   0        0        0      372 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcp_leases.textfsm
+-rw-r--r--   0        0        0      270 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcpv6_server_leases.textfsm
+-rw-r--r--   0        0        0      293 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces.textfsm
+-rw-r--r--   0        0        0      307 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces_ethernet_physical.textfsm
+-rw-r--r--   0        0        0      662 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm
+-rw-r--r--   0        0        0      233 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      471 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      380 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_version.textfsm
+-rw-r--r--   0        0        0      314 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgeswitch_show_arp.textfsm
+-rw-r--r--   0        0        0      553 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm
+-rw-r--r--   0        0        0      209 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgeswitch_show_vlan.textfsm
+-rw-r--r--   0        0        0      470 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vmware_nsxv_show_ip_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0      259 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vmware_nsxv_show_ip_route.textfsm
+-rw-r--r--   0        0        0      281 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vyatta_vyos_show_arp.textfsm
+-rw-r--r--   0        0        0      374 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vyatta_vyos_show_interfaces.textfsm
+-rw-r--r--   0        0        0      859 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0      231 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/watchguard_firebox_show_arp.textfsm
+-rw-r--r--   0        0        0     1181 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/yamaha_show_environment.textfsm
+-rw-r--r--   0        0        0      472 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/yamaha_show_ip_route.textfsm
+-rw-r--r--   0        0        0      626 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm
+-rw-r--r--   0        0        0      402 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_intf_group_get.textfsm
+-rw-r--r--   0        0        0      563 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm
+-rw-r--r--   0        0        0      409 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_lan_get.textfsm
+-rw-r--r--   0        0        0      662 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm
+-rw-r--r--   0        0        0      411 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_lanhosts_get.textfsm
+-rw-r--r--   0        0        0      664 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm
+-rw-r--r--   0        0        0      751 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm
+-rw-r--r--   0        0        0      629 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm
+-rw-r--r--   0        0        0      339 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_static_dhcp_get.textfsm
+-rw-r--r--   0        0        0      625 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm
+-rw-r--r--   0        0        0      539 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm
+-rw-r--r--   0        0        0      857 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm
+-rw-r--r--   0        0        0      337 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_zycli_Ethctl_media-type.textfsm
+-rw-r--r--   0        0        0     3098 2023-06-11 21:19:43.932714 ntc_templates-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3871 1970-01-01 00:00:00.000000 ntc_templates-3.4.0/PKG-INFO
```

### Comparing `ntc_templates-3.3.0/LICENSE` & `ntc_templates-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/README.md` & `ntc_templates-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/parse.py` & `ntc_templates-3.4.0/ntc_templates/parse.py`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_port.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_port.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Value Required INTERFACE (\S+)
 Value LINK_STATUS (.*)
 Value PROTOCOL_STATUS (.*)
 Value HARDWARE_TYPE ([\w+-]+)
 Value ADDRESS ([a-zA-Z0-9]+.[a-zA-Z0-9]+.[a-zA-Z0-9]+)
 Value BIA ([a-zA-Z0-9]+.[a-zA-Z0-9]+.[a-zA-Z0-9]+)
-Value DESCRIPTION (.*)
+Value DESCRIPTION ([^\"]*)
 Value IP_ADDRESS (\d+\.\d+\.\d+\.\d+\/\d+)
 Value MTU (\d+)
 Value BANDWIDTH (\d+\s+\w+)
 Value INTERFACE_UP_TIME (.*)
 Value LINK_STATUS_CHANGE (\d+)
 
 Start
   ^\S+\s+is\s+\S+,\s+line\s+protocol\s+is\s+\S+\s+\S+ -> Continue.Record
   ^${INTERFACE}\s+is\s+${LINK_STATUS},\s+line\s+protocol\s+is\s+${PROTOCOL_STATUS}
   ^\s+Hardware\s+is\s+${HARDWARE_TYPE}(.*address\s+is\s+${ADDRESS})*(.*bia\s+${BIA})*
-  ^\s+Description:\s+${DESCRIPTION}
+  ^\s+Description:\s+"?${DESCRIPTION}"?$$
   ^\s+Internet\s+address\s+is\s+${IP_ADDRESS}
   ^\s+(Up|Down)\s+${INTERFACE_UP_TIME}
   ^\s+${LINK_STATUS_CHANGE}\s+link\s+status\s+changes.*
   ^.*MTU\s+${MTU}(.*BW\s+${BANDWIDTH})*
   ^\s*
   ^. -> Error
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_inventory.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_inventory.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_module.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_module.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_vlan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/arista_eos_show_vrf.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/aruba_os_show_arp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/broadcom_icos_show_version.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_span.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_span.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_port_show.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_port_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_software_show.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_software_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_dir.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_dir.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_ping.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_ping.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_failover.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_failover.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_logging.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_logging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_nat.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_nat.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_version.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_ping.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_ping.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # IOS ACL structure is quite complex.
-# 
+#
 # Extended IP ACL:
 # 	SEQUENCE_NUMBER ACTION PROTOCOL SOURCE [PORT id] [RANGE start finish] DESTINATION [MODIFIER]
 #
 # Standard ACL:
 #	SEQUENCE_NUMBER ACTION SOURCE DESTINATION [MODIFIER]
-#	 
+#
 #
 Value Filldown NAME (\S+)
 Value Required SN (\d+)
 Value ACTION (\w+)
 Value PROTOCOL (\w+)
 #
 # SOURCE RegEx must be able to catch every possible source combination including masks. 'any' and 'host' and 'wildcard bits' are possible too.
@@ -21,19 +21,22 @@
 Value PORT (eq|gt|lt|neq|range)
 #
 # This can be either a single port or a list.
 #
 Value RANGE ([(\S+\s\S+)]+)
 #
 # DESTINATION RegEx must be able to catch every possible source combination including masks. 'any' and 'host' and 'wildcard bits' are possible too.
-# 
+#
 Value DESTINATION (host\s\d+\.\d+\.\d+\.\d+|any|\d+\.\d+\.\d+\.\d+\s\d+\.\d+\.\d+\.\d+|\d+\.\d+\.\d+\.\d+,\s+wildcard bits\s\d+\.\d+\.\d+\.\d+)
-Value MODIFIER (.*)
+# MODIFIER "eq ftp" | "log" | "gt 1024"
+Value MODIFIER ((\w+\s)?\w+)
+Value MATCHES (\d+)
 
 Start
   ^.*list\s+${NAME}
   ^\s+${SN}\s+${ACTION}\s+${PROTOCOL}\s+${SOURCE}(\s+${PORT})*(\s${RANGE})*\s+${DESTINATION}(\s+${MODIFIER})* -> Record
-  ^\s+${SN}\s+${ACTION}\s+${SOURCE}(\s+${MODIFIER})* -> Record
+  ^\s*${SN}\s+${ACTION}\s+${SOURCE}(\s+${MODIFIER}(\s\(${MATCHES} matches\))?)? -> Record
   # Capture time-stamp if vty line has command time-stamping turned on
   ^Load\s+for\s+
   ^Time\s+source\s+is
-
+  ^\s*$$
+  ^. -> Error
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_archive.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_archive.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_boot.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_boot.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Value Required CERTIFICATE_TYPE ([CA]*\s*Certificate)
 Value STATUS ([\s\S]+?)
 Value SERIAL_NUMBER (\S+)
 Value CERTIFICATE_USAGE ([\s\S]+?)
 Value ISSUER_E (\S+)
-Value ISSUER_CN (\S+)
-Value ISSUER_OU (\S+)
-Value ISSUER_O (\S+)
-Value ISSUER_L (\S+)
-Value ISSUER_ST (\S+)
-Value ISSUER_C (\S+)
+Value ISSUER_CN ([\s\S]+)
+Value ISSUER_OU ([\s\S]+)
+Value ISSUER_O ([\s\S]+)
+Value ISSUER_L ([\s\S]+)
+Value ISSUER_ST ([\s\S]+)
+Value ISSUER_C ([\s\S]+)
 Value SUBJECT_E (\S+)
-Value SUBJECT_CN (\S+)
-Value SUBJECT_OU (\S+)
-Value SUBJECT_O (\S+)
-Value SUBJECT_L (\S+)
-Value SUBJECT_ST (\S+)
-Value SUBJECT_C (\S+)
+Value SUBJECT_CN ([\s\S]+)
+Value SUBJECT_OU ([\s\S]+)
+Value SUBJECT_O ([\s\S]+)
+Value SUBJECT_L ([\s\S]+)
+Value SUBJECT_ST ([\s\S]+)
+Value SUBJECT_C ([\s\S]+)
 Value SUBJECT_NAME (\S+)
 Value SUBJECT_SERIAL_NUMBER (\S+)
 Value SUBJECT_HOSTNAME (\S+)
 Value CRL_DISTRIBUTION_POINT (\S+)
 Value START_DATE ([\s\S]+?)
 Value END_DATE ([\s\S]+?)
 Value RENEW_DATE ([\s\S]+?)
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Value ADDRESS ([a-fA-F0-9]{4}\.[a-fA-F0-9]{4}\.[a-fA-F0-9]{4})
 Value BIA ([a-fA-F0-9]{4}\.[a-fA-F0-9]{4}\.[a-fA-F0-9]{4})
 Value DESCRIPTION (.+?)
 Value IP_ADDRESS (\d+\.\d+\.\d+\.\d+\/\d+)
 Value MTU (\d+)
 Value DUPLEX (([Ff]ull|[Aa]uto|[Hh]alf|[Aa]-).*?)
 Value SPEED (.*?)
-Value MEDIA_TYPE (\S+(\s+\S+)?)
+Value MEDIA_TYPE (\S+.*)
 Value BANDWIDTH (\d+\s+\w+)
 Value DELAY (\d+\s+\S+)
 Value ENCAPSULATION (.+?)
 Value LAST_INPUT (.+?)
 Value LAST_OUTPUT (.+?)
 Value LAST_OUTPUT_HANG (.+?)
 Value QUEUE_STRATEGY (.+)
@@ -45,14 +45,16 @@
   ^\s+MTU\s+${MTU}.*BW\s+${BANDWIDTH}.*DLY\s+${DELAY},\s*$$
   ^\s+Encapsulation\s+${ENCAPSULATION}, Vlan ID\s+${VLAN_ID}.+$$
   ^\s+Encapsulation\s+${ENCAPSULATION}, outer ID\s+${VLAN_ID_OUTER}, inner ID\s+${VLAN_ID_INNER}.+$$
   ^\s+Encapsulation\s+${ENCAPSULATION},.+$$
   ^\s+Last\s+input\s+${LAST_INPUT},\s+output\s+${LAST_OUTPUT},\s+output\s+hang\s+${LAST_OUTPUT_HANG}\s*$$
   ^\s+Queueing\s+strategy:\s+${QUEUE_STRATEGY}\s*$$
   ^\s+${DUPLEX},\s+${SPEED},.+media\stype\sis\s${MEDIA_TYPE}$$
+  ^\s+${DUPLEX},\s+${SPEED},.+TX/FX$$
+  ^\s+${DUPLEX},\s+${SPEED}$$
   ^.*input\s+rate\s+${INPUT_RATE}\s+\w+/sec,\s+${INPUT_PPS}\s+packets.+$$
   ^.*output\s+rate\s+${OUTPUT_RATE}\s+\w+/sec,\s+${OUTPUT_PPS}\s+packets.+$$
   ^\s+${INPUT_PACKETS}\s+packets\s+input,\s+\d+\s+bytes,\s+\d+\s+no\s+buffer\s*$$
   ^\s+${RUNTS}\s+runts,\s+${GIANTS}\s+giants,\s+\d+\s+throttles\s*$$
   ^\s+${INPUT_ERRORS}\s+input\s+errors,\s+${CRC}\s+CRC,\s+${FRAME}\s+frame,\s+${OVERRUN}\s+overrun,\s+\d+\s+ignored\s*$$
   ^\s+${INPUT_ERRORS}\s+input\s+errors,\s+${CRC}\s+CRC,\s+${FRAME}\s+frame,\s+${OVERRUN}\s+overrun,\s+\d+\s+ignored,\s+${ABORT}\s+abort\s*$$
   ^\s+${OUTPUT_PACKETS}\s+packets\s+output,\s+\d+\s+bytes,\s+\d+\s+underruns\s*$$
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Value Filldown TYPE (\w{0,2})
 Value Required,Filldown NETWORK (\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3})
 Value Filldown MASK (\d{1,2})
 Value DISTANCE (\d+)
 Value METRIC (\d+)
 Value NEXTHOP_IP (\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3})
 Value NEXTHOP_VRF (\S+)
-Value NEXTHOP_IF ([A-Z][\w\-\.:/]+)
+Value NEXTHOP_IF ([A-Za-z][\w\-\.:/]+)
 Value UPTIME (\d[\w:\.]+)
 
 Start
   ^Routing\sTable:\s${VRF}\s*$$
   ^Gateway.* -> Routes
   # Capture time-stamp if vty line has command time-stamping turned on
   ^Load\s+for\s+
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_license.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_license.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 Value NEIGHBOR_INTERFACE (.*)
 Value NEIGHBOR (.+?)
 Value SYSTEM_DESCRIPTION (.*)
 Value CAPABILITIES (.*)
 Value MANAGEMENT_IP (\S+)
 Value VLAN (\d+)
 Value SERIAL (\S+)
+Value MANUFACTURER (.*)
+Value HW_REVISION (\S+)
+Value FW_REVISION (\S+)
+Value SW_REVISION (\S+)
+Value MODEL (.*)
 Value POWER_PAIR (\S+)
 Value POWER_CLASS (\d+)
 Value POWER_DEVICE_TYPE (\S+)
 Value POWER_PRIORITY (\S+)
 Value POWER_SOURCE (\S+)
 Value POWER_REQUESTED (\d+)
 
@@ -77,13 +82,18 @@
   ^\s+Power\s+Source:\s+${POWER_SOURCE}\s*$$
   ^\s+Power\s+Priority:\s+${POWER_PRIORITY}\s*$$
   ^\s+Power\s+Requested:\s+${POWER_REQUESTED}\s+mW\s*$$
   ^\s*$$ -> Start
 
 Med
   ^\s+Serial\s+number:\s+${SERIAL}\s*$$
+  ^\s+Manufacturer:\s+${MANUFACTURER}\s*$$
+  ^\s+Model:\s+${MODEL}\s*$$
+  ^\s+H/W revision:\s+${HW_REVISION}\s*$$
+  ^\s+F/W revision:\s+${FW_REVISION}\s*$$
+  ^\s+S/W revision:\s+${SW_REVISION}\s*$$
   ^\s+\S+
   ^\s*$$
   ^\s*Total\s+entries\s+displayed -> Record
   ^\s*-+\s*$$ -> Continue.Record
   ^\s*-+\s*$$ -> Start
   ^.* -> Error
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_logging.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_logging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_module.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Value AGING_TIME (\d{1,4}\smins)
 Value AGING_TYPE ([Aa]bsolute|[Ii]nactivity)
 Value SS_ADDR_AGING (\w+)
 Value MAX_MAC_ADDRS (\d+)
 Value TOTAL_MAC_ADDRS (\d+)
 Value CONFIG_MAC_ADDRS (\d+)
 Value STICKY_MAC_ADDRS (\d+)
-Value LAST_SRC_MAC_ADDR_VLAN (\d.+:\d+)
+Value LAST_SRC_MAC_ADDR_VLAN (\w.+:\d+)
 Value VIOLATION_COUNT (\d+)
 
 Start
   ^Port Security\s+:\s+${PORT_SECURITY}
   ^Port Status\s+:\s+${PORT_STATUS}
   ^Violation Mode\s+:\s+${VIOLATION_MODE}
   ^Aging Time\s+:\s+${AGING_TIME}
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_standby.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_standby.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_version.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_ios_traceroute.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_traceroute.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # NX-OS ACL structure is quite complex and includes IP, IPv6 and MAC ACL types.
-# 
+#
 # IP/IPv6 ACL:
 # 	SEQUENCE_NUMBER ACTION PROTOCOL SOURCE [PORT id] [RANGE start finish] DESTINATION [MODIFIER]
 #
 # MAC ACL:
 #	SEQUENCE_NUMBER ACTION SOURCE DESTINATION [MODIFIER]
-#	 
+#
 Value Filldown NAME (.*)
 Value Required SN (\d+)
 Value ACTION (\w+)
 Value PROTOCOL ([^any][\w+\d+]+)
-# SOURCE RegEx must be able to catch both MAC and IP addresses including masks. 'any' and 'address group' are possible too. 
+# SOURCE RegEx must be able to catch both MAC and IP addresses including masks. 'any' and 'address group' are possible too.
 Value SOURCE ([\w+\d+]+\.[\w+\d+]+\.[\w+\d+]+\s[\w+\d+]+\.[\w+\d+]+\.[\w+\d+]+|any|\d+\.\d+\.\d+\.\d+/\d+|addrgroup\s\S+|\S+)
 # RANGE RegEx catches the first and last protocol to match in the interval range.
 Value RANGE (\S+\s\S+)
 # We can specify protocols to match. 'eq', 'gt', 'lt' and 'neq' are supported.
 Value PORT (eq\s\S+|gt\s\S+|lt\s\S+|neq\s\S+)
 # SOURCE RegEx must be able to catch both MAC and IP addresses including masks. 'any' and 'address group' are possible too.
 Value DESTINATION ([\w+\d+]+\.[\w+\d+]+\.[\w+\d+]+\s[\w+\d+]+\.[\w+\d+]+\.[\w+\d+]+|any|\d+\.\d+\.\d+\.\d+/\d+|addrgroup\s\S+|\S+)
-# What it remains is some ACL modifier used to do fancy stuff. 
+# What it remains is some ACL modifier used to do fancy stuff.
 Value MODIFIER (.*)
+Value REMARK (.*)
 
 Start
-  # ACL name is catched. This is a FILLDOWN value, so everyother line without a NAME would inherits the last value matched.
-  ^.*list\s+${NAME} 
+  # ACL name is matched not starting with space. FILLDOWN, other line's inherit last NAME
+  ^[^\s].*\slist\s+${NAME}$$
+  # Catch remarks as uniq type, capture Action first and then Action=remark
+  ^\s+${SN}\s+${ACTION}\s -> Continue
+  ^\s+${SN}\s+remark\s${REMARK}$$ -> Record
   # This line matches all the possible combination of fields specifed above.
   ^\s+${SN}\s+${ACTION}(\s+${PROTOCOL})*\s+${SOURCE}(\s+${PORT})*(\s+range\s${RANGE})*\s+${DESTINATION}(\s+${MODIFIER})* -> Record
-
+  # Drop lines we are not interested in
+  ^\s+statistics per-entry
+  ^\s*$$
+  ^. -> Error
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-Value INTERFACE ([\w+/]+)
+Value INTERFACE ([\w+/\.]+)
 Value VRF (\S+)
 Value STATUS (up|down)
-Value IP (\d+\.\d+\.\d+\.\d+)
+Value IP (\S+)
 Value SPEED (\S+)
 Value MTU (\d+)
 Value VLAN ([\d+-]+)
 Value TYPE (\S+)
-Value MODE (routed|access|trunk|pvlan|fabric)
+Value MODE (\S+)
 Value REASON (\S+((\s\w+)+)?)
 Value PORTCH (\S+)
 Value DESCRIPTION (\S+((\s\w+)+)?)
 Value PROTOCOL (\S+)
 
 Start
-  ^Port\s+VRF\s+Status\s+IP\s+Address\s+Speed\s+MTU -> Management 
+  ^Port\s+VRF\s+Status\s+IP\s+Address\s+Speed\s+MTU -> Management
   ^Ethernet\s+VLAN\s+Type\sMode\s+Status\s+Reason\s+Speed\s+Port\s*$$ -> Ethernet
-  ^Interface\s+Ch\s+ -> Ethernet 
+  ^Interface\s+Ch\s+ -> Ethernet
   ^Interface\s+Status\s+Description\s*$$ -> Loopback
   ^Interface\s+Secondary\s+VLAN\(Type\)\s+Status\s+Reason -> VLAN
   ^Port-channel\s+VLAN\s+Type\sMode\s+Status\s+Reason\s+Speed\s+Protocol -> PORTCHANNEL
+  ^Interface\s+Status\s+IP\s+Address\s+Encap\s+type\s+MTU -> TUNNEL
   ^---+$$
   ^. -> Error Start
 
 Management
   ^${INTERFACE}\s+${VRF}\s+${STATUS}\s+${IP}\s+${SPEED}\s+${MTU} -> Record
   ^Ethernet\s+VLAN\s+Type\s+Mode\s+Status\s+Reason\s+Speed\s+Port -> Start
   ^---+$$
@@ -50,7 +51,13 @@
 
 PORTCHANNEL
   ^Interface\s*$$
   ^${INTERFACE}\s+${VLAN}\s+${TYPE}\s+${MODE}\s+${STATUS}\s+${REASON}\s+${SPEED}\s+${PROTOCOL} -> Record
   ^---+$$
   ^\s*$$ -> Start
   ^. -> Error PORTCHANNEL
+
+TUNNEL
+  ^${INTERFACE}\s+${STATUS}\s+${IP}\s+${TYPE}\s+${MTU} -> Record
+  ^---+$$
+  ^\s*$$ -> Start
+  ^. -> Error TUNNEL
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_version.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_arp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/cisco_xr_show_version.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/dell_force10_show_vlan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_system_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/fortinet_get_system_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_interface.textfsm`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,23 @@
   ^\s*Line\s+protocol\s+state:\s+${PROTOCOL_STATUS}
   ^\s*Line\s+protocol\s+current\s+state:\s+${PROTOCOL_STATUS}
   ^\s*Description:\s+${DESCRIPTION}
   ^\s*Bandwidth:\s+${BANDWIDTH}
   ^\s*Maximum\s+[Tt]ransmi\S+\s+[Uu]nit:\s+${MTU}
   ^\s*The\sMaximum\s+Transmit\s+Unit\sis\s+${MTU}
   ^\s*Maximum\s+frame\s+length:\s+${L2MTU}
+  ^\s*Forbid\s+jumbo\s+frames\s+to\s+pass
   ^\s*The\sMaximum\s+Frame\s+Length\sis\s+${L2MTU}
   ^\s*Internet\s+[Aa]ddress:\s+${IP_ADDRESS}\s+\([Pp]rimary\)
   ^\s*Internet\s+[Aa]ddress\sis\s+${IP_ADDRESS}\s+[Pp]rimary
   ^\s*Internet\s+[Aa]ddress:\s+${IP_ADDRESS}\s+\([Ss]ub\)
   ^\s*IP\s+[Pp]acket\s+[Ff]rame\s+[Tt]ype\s*:\s*[^,]+,\s+[Hh]ardware\s+[Aa]ddress:\s+${HW_ADDRESS}
   ^\s*IPv6\s+[Pp]acket\s+[Ff]rame\s+[Tt]ype\s*:\s*[^,]+,\s+[Hh]ardware\s+[Aa]ddress:\s+${HW_ADDRESS}
   ^\s*${SPEED}\s+mode,\s+${DUPLEX}\s+mode
-  ^\s*${SPEED},\s+${DUPLEX},\s+link\s+type:\s+\S+,
+  ^\s*${SPEED},\s+${DUPLEX},\s+link\s+type
   ^\s*PVID:\s+${VLAN_NATIVE}
   ^\s*Port\s+link-type:\s+${PORT_LINK_TYPE}
   # Trunk - Passing VLANs (parsing multiple times with Continue)
   ^\s+VLAN\s+[Pp]assing\s*:\s+${VLAN_PASSING},* -> Continue
   # Skip initial VLANs and read the Nth + 1
   ^\s+VLAN\s+[Pp]assing\s*:(?:\s+[^,]+,){1}\s+${VLAN_PASSING},* -> Continue
   ^\s+VLAN\s+[Pp]assing\s*:(?:\s+[^,]+,){2}\s+${VLAN_PASSING},* -> Continue
@@ -130,14 +131,16 @@
   # End od VLAN Passing
   ^\s+VLAN\s+permitted:
   ^\s{14,}
   # Next
   ^$$ -> Next.Record
   # Drop
   ^\s*Link
+  ^\s*Encapsulation\s+is
+  ^\s*Phy-mru
   ^\s*Last
   ^\s*Trunk\s+port
   ^\s*Loopback
   ^\s*Media
   ^\s*[Ff]low
   ^\s*Allow\s+jumbo
   ^\s*Broadcast
@@ -154,22 +157,30 @@
   ^\s+Un[tT]agged\s+VLAN
   ^\s*[Ii]nput
   ^\s*[Oo]utput
   ^\s*Physical
   ^\s*Internet\s+protocol
   ^\s*Port\s+hardware
   ^\s+\d+\s+unicasts
+  ^\s+-\s+unicasts
   ^\s+\d+\s+[Cc][Rr][Cc]
   ^\s+\d+\s+aborts
-  ^\s+\d+\s+packets,*\s+
-  ^\s+\d+\s+errors,*\s+
+  ^\s+\d+\s+packets,*\s*
+  ^\s+\d+\s+errors,*\s*
   ^\s+\d+\s+lost
-  ^\s+\d+\s+drops,*\s+
-  ^\s+\d+\s+deferred,*\s+
+  ^\s+\d+\s+input\s+error
+  ^\s+\d+\s+output\s+error
+  ^\s+\d+\s+drops,*\s*
+  ^\s+\d+\s+deferred,*\s*
   ^\s+\d+\s+broadcasts
   ^\s+\d+\s+ignored
+  ^\s+\d+\s+dribbles
+  ^\s*Tunnel\s
+  ^\s*GRE
+  ^\s*Checksumming\sof\sGRE
   ^\s+-\s+ignored
   ^\s+-\s+frame
   ^\s+-\s+aborts
   ^\s+-\s+lost\s+carrier
+  ^\s*DCD:
   ^. -> Error
   ^\s*$$ ^. -> Error
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Value INTF (\S+)
 Value LINE_STATUS (UP|DOWN|Administratively DOWN)
 Value PROTOCOL_STATUS (UP(\(spoofing\))?|DOWN)
+Value ROUTE_MAP (\S+)
 Value List IPADDR (\S+)
 Value MTU (\d+)
 
 
 Start
   ^${INTF}\s+current\s+state\s*:\s*${LINE_STATUS} -> Interface
   ^. -> Error
@@ -14,14 +15,15 @@
   ^\S+\s+current\s+state -> Continue.Record
   ^${INTF}\s+current\s+state\s*:\s*${LINE_STATUS}
   ^Line\s+protocol\s+current\s+state\s*:\s*${PROTOCOL_STATUS}
   ^Internet\s+Address\s+is\s+${IPADDR}\s+Primary
   ^Internet\s+Address\s+is\s+${IPADDR}\s+Sub
   ^Broadcast\s+address\s*:\s*\S+
   ^The\s+Maximum\s+Transmit\s+Unit\s*:\s*${MTU}\s+bytes
+  ^Policy\s+routing\s+is\s+enabled,\s+using\s+route\s+map\s+${ROUTE_MAP}
   ^input\spackets\s*:\s*\d+,\sbytes\s*:\s*\d+,\smulticasts\s*:\s*\d+
   ^output\spackets\s*:\s*\d+,\sbytes\s*:\s*\d+,\smulticasts\s*:\s*\d+
   ^TTL\sinvalid\spacket\snumber\s*:\s*\d+
   ^ICMP\spacket\sinput\snumber\s*:\s*\d+
   ^ARP\spacket\sinput\snumber\s*:\s*\d+
   ^\s+Echo\sreply\s*:\s*\d+
   ^\s+Unreachable\s*:\s*\d+
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 Value ROUTE_INTERFACE (.*)
 Value IPV4_ADDRESS (\S+)
 Value IPV4_SUBNET (\S+)
 
 Start
   ^\s*VLAN\s+ID\s*: -> Continue.Record
   ^\s*VLAN\s+ID\s*:\s*${VLAN_ID}
-  ^\s*VLAN\s+type\s*:\s*${TYPE}
-  ^\s*Route\s+interface\s*:\s*${ROUTE_INTERFACE}
-  ^\s*IPv4\s+address\s*:\s*${IPV4_ADDRESS}
-  ^\s*IPv4\s+subnet\s+mask\s*:\s*${IPV4_SUBNET}
+  ^\s*VLAN\s+[Tt]ype\s*:\s*${TYPE}
+  ^\s*Route\s+[Ii]nterface\s*:\s*${ROUTE_INTERFACE}
+  ^\s*IPv4\s+[Aa]ddress\s*:\s*${IPV4_ADDRESS}
+  ^\s*IPv4\s+[Ss]ubnet\s+mask\s*:\s*${IPV4_SUBNET}
   ^\s*Description\s*:\s*${DESCRIPTION}
   ^\s*Name\s*:\s*${NAME}
-  ^\s*Tagged\sports
-  ^\s*Untagged\sports
+  ^\s*Tagged\s+[Pp]orts
+  ^\s*Untagged\s+[Pp]orts
   ^\s{3,}\S+\s*$$
   ^\s{3,}\S+\s+\S+\s*$$
+  ^\s{3,}\S+\s+\S+\s+\S+\s*$$
   ^. -> Error
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/hp_procurve_show_system.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_system.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Value Filldown ACL_NAME (.*?)
-Value Filldown ACL_NUMBER (\d+)
-Value Required SN (\d+)
+Value Filldown,Required ACL_NUMBER (\d+)
+Value SN (\d+)
 Value ACTION (deny|permit)
 Value PROTOCOL (\d+|icmp(v6)?|tcp|udp|gre|igmp|ip(v6)?|ipinip|ospf)
 Value SOURCE (((\d+.){3}\d+|[0-9a-fA-F]{1,4}([0-9a-fA-F]{0,4}:){1,7}[0-9a-fA-F]{0,4})[\/\s]((\d+.){3}\d+|\d+))
 Value SOURCE_PORT_MODIFIER (eq|lt|gt|range)
-Value SOURCE_PORT_RANGE ((\d+)(\s(\d+))?)
+Value SOURCE_PORT_RANGE ((\S+)(\s(\S+))?)
 Value DESTINATION (((\d+.){3}\d+|[0-9a-fA-F]{1,4}([0-9a-fA-F]{0,4}:){1,7}[0-9a-fA-F]{0,4})[\/\s]((\d+.){3}\d+|\d+))
 Value DESTINATION_PORT_MODIFIER (eq|lt|gt|range)
-Value DESTINATION_PORT_RANGE ((\d+)(\s(\d+))?)
+Value DESTINATION_PORT_RANGE ((\S+)(\s(\S+))?)
 Value MATCHES (\d+)
+Value DESCRIPTION (.*)
 
 Start
+  ^\s*rule\s\d+\s(deny|permit) -> Continue.Record
+  ^\S+\sIPv6\sACL\s -> Continue.Record
+  ^\S+\sACL\s -> Continue.Record
   ^\s*Total\squantity\sof\snonempty\sACL\snumber\sis\s\d+\s*$$
   ^\s*Total\snonempty\sacl6\snumber\sis\s\d+\s*$$
-  ^\S+(\sIPv6)?\sACL\s(${ACL_NAME}\s)?${ACL_NUMBER},\s\d+.*$$
+  ^\S+\sIPv6\sACL\s${ACL_NUMBER}(\sname\s${ACL_NAME})?,\s\d+\srules?.*$$
+  ^\S+\sACL\s(${ACL_NAME}\s)?${ACL_NUMBER},\s\d+\srules?.*$$
   ^\s*Acl's\sstep\sis\s\d+\s*$$
-  ^\s*rule\s${SN}\s${ACTION}(\s${PROTOCOL})?(\ssource\s${SOURCE})?(\ssource-port\s${SOURCE_PORT_MODIFIER}\s${SOURCE_PORT_RANGE})?(\sdestination\s${DESTINATION})?(\sdestination-port\s${DESTINATION_PORT_MODIFIER}\s${DESTINATION_PORT_RANGE})?(\s\(${MATCHES}\smatch(es)?\))?\s*$$ -> Record
+  ^\s*rule\s${SN}\s${ACTION}(\s${PROTOCOL})?(\ssource\s${SOURCE})?(\ssource-port\s${SOURCE_PORT_MODIFIER}\s${SOURCE_PORT_RANGE})?(\sdestination\s${DESTINATION})?(\sdestination-port\s${DESTINATION_PORT_MODIFIER}\s${DESTINATION_PORT_RANGE})?(\s\(${MATCHES}\smatch(es)?\))?\s*$$
+  ^\s*rule\s\d+\sdescription\s"${DESCRIPTION}"\s*$$
   ^\s*$$
   ^. -> Error
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/index` & `ntc_templates-3.4.0/ntc_templates/templates/index`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,15 @@
 cisco_ios_show_isdn_status.textfsm, .*, cisco_ios, sh[[ow]] isd[[n]] st[[atus]]
 cisco_ios_show_ap_summary.textfsm, .*, cisco_ios, sh[[ow]] ap sum[[mary]]
 cisco_ios_show_dhcp_lease.textfsm, .*, cisco_ios, sh[[ow]] dh[[cp]] l[[ease]]
 cisco_ios_show_interfaces.textfsm, .*, cisco_ios, sh[[ow]] int[[erfaces]](?: (?:\S+))?
 cisco_ios_show_ipv6_route.textfsm, .*, cisco_ios, sh[[ow]] ipv6 r[[oute]]
 cisco_ios_show_redundancy.textfsm, .*, cisco_ios, sh[[ow]] redu[[ndancy]]
 cisco_ios_show_snmp_group.textfsm, .*, cisco_ios, sh[[ow]] snm[[p]] g[[roup]]
+cisco_ios_show_vrf_detail.textfsm, .*, cisco_ios, sh[[ow]] vrf detail
 cisco_ios_show_vrrp_brief.textfsm, .*, cisco_ios, sh[[ow]] vrr[[p]] b[[rief]]
 cisco_ios_show_vtp_status.textfsm, .*, cisco_ios, sh[[ow]] vtp stat[[us]]
 cisco_ios_show_adjacency.textfsm, .*, cisco_ios, sh[[ow]] ad[[jacency]]
 cisco_ios_show_dot1x_all.textfsm, .*, cisco_ios, sh[[ow]] dot1x a[[ll]]
 cisco_ios_show_inventory.textfsm, .*, cisco_ios, sh[[ow]] inven[[tory]]
 cisco_ios_show_ip_mroute.textfsm, .*, cisco_ios, sh[[ow]] ip mr[[oute]]
 cisco_ios_show_nve_peers.textfsm, .*, cisco_ios, sh[[ow]] nv[[e]] p[[eers]]
@@ -301,35 +302,41 @@
 cisco_ios_show_boot.textfsm, .*, cisco_ios, sh[[ow]] boot
 cisco_ios_show_vlan.textfsm, .*, cisco_ios, sh[[ow]] vlan
 cisco_ios_show_vrf.textfsm, .*, cisco_ios, sh[[ow]] vrf
 cisco_ios_ping.textfsm, .*, cisco_ios, ping
 cisco_ios_dir.textfsm,  .*, cisco_ios, dir
 
 cisco_nxos_show_l2rib_internal_permanently-frozen-list.textfsm, .*, cisco_nxos, sh[[ow]] l2ri[[b]] i[[nternal]] pe[[rmanently-frozen-list]]
+cisco_nxos_show_ip_pim_interface_brief_vrf_all.textfsm, .*, cisco_nxos, sh[[ow]] ip pim int[[erface]] br[[ief]] vrf all
 cisco_nxos_show_configuration_session_summary.textfsm, .*, cisco_nxos, sh[[ow]] configu[[ration]] s[[ession]] su[[mmary]]
 cisco_nxos_show_interface_transceiver_details.textfsm, .*, cisco_nxos, sh[[ow]] int[[erface]] tra[[nsceiver]] de[[tails]]
 cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm, .*, cisco_nxos, sh[[ow]] ip dh[[cp]] sn[[ooping]] st[[atistics]]
+cisco_nxos_show_ip_pim_group-range_vrf_all.textfsm, .*, cisco_nxos, sh[[ow]] ip pim group[[-range]] vrf all
 cisco_nxos_show_environment_temperature.textfsm, .*, cisco_nxos, sh[[ow]] env[[ironment]] t[[emperature]]
+cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm, .*, cisco_nxos, sh[[ow]] ip msdp summary vrf all
 cisco_nxos_show_ip_ospf_interface_brief.textfsm, .*, cisco_nxos, sh[[ow]] ip ospf int[[erface]] b[[rief]](?: vrf \S+)?\s*$
+cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm, .*, cisco_nxos, sh[[ow]] ip pim nei[[ghbor]] vrf all
 cisco_nxos_show_forwarding_ipv4_route.textfsm, .*, cisco_nxos, sh[[ow]] fo[[rwarding]] ipv4 ro[[ute]]
 cisco_nxos_show_interface_description.textfsm, .*, cisco_nxos, sh[[ow]] int[[erface]] desc[[ription]]
 cisco_nxos_show_interface_transceiver.textfsm, .*, cisco_nxos, sh[[ow]] int[[erface]] tra[[nsceiver]]
 cisco_nxos_show_interfaces_switchport.textfsm, .*, cisco_nxos, sh[[ow]] int[[erfaces]] sw[[itchport]]
 cisco_nxos_show_ip_dhcp_relay_address.textfsm, .*, cisco_nxos, sh[[ow]] ip dh[[cp]] r[[elay]] a[[ddress]]
 cisco_nxos_show_lldp_neighbors_detail.textfsm, .*, cisco_nxos, sh[[ow]] ll[[dp]] nei[[ghbors]] d[[etail]]
 cisco_nxos_show_cdp_neighbors_detail.textfsm, .*, cisco_nxos, sh[[ow]] c[[dp]] neig[[hbors]] det[[ail]]
 cisco_nxos_show_forwarding_adjacency.textfsm, .*, cisco_nxos, sh[[ow]] fo[[rwarding]] (?:ipv4 )?ad[[jacency]]
 cisco_nxos_show_ip_interface_vrf_all.textfsm, .*, cisco_nxos, sh[[ow]] ip interf[[ace]] v[[rf]] a[[ll]]
 cisco_nxos_show_ipv6_interface_brief.textfsm, .*, cisco_nxos, sh[[ow]] ipv[[6]] interf[[ace]] b[[rief]]
 cisco_nxos_show_port-channel_summary.textfsm, .*, cisco_nxos, sh[[ow]] po[[rt-channel]] sum[[mary]]
 cisco_nxos_show_cts_interface_brief.textfsm, .*, cisco_nxos, sh[[ow]] cts inte[[rface]] br[[ief]]
 cisco_nxos_show_ip_bgp_summary_vrf.textfsm, .*, cisco_nxos, sh[[ow]] ip b[[gp]] s[[ummary]] v[[rf]]
 cisco_nxos_show_ip_interface_brief.textfsm, .*, cisco_nxos, sh[[ow]] ip int[[erface]] b[[rief]](?: vrf \S+)?\s*$
+cisco_nxos_show_spanning-tree_root.textfsm, .*, cisco_nxos, sh[[ow]] sp[[an]]ning-tree root
 cisco_nxos_show_cts_interface_all.textfsm, .*, cisco_nxos, sh[[ow]] ct[[s]] inter[[face]] al[[l]]
 cisco_nxos_show_ip_community-list.textfsm, .*, cisco_nxos, sh[[ow]] ip comm[[unity-list]]
+cisco_nxos_show_ip_pim_rp_vrf_all.textfsm, .*, cisco_nxos, sh[[ow]] ip pim rp vrf all
 cisco_nxos_show_mac_address-table.textfsm, .*, cisco_nxos, sh[[ow]] m[[ac]] addr[[ess-table]]
 cisco_nxos_show_interface_status.textfsm, .*, cisco_nxos, sh[[ow]] int[[erface]] st[[atus]]
 cisco_nxos_show_ip_bgp_neighbors.textfsm, .*, cisco_nxos, sh[[ow]] ip bgp nei[[ghbors]]
 cisco_nxos_show_ip_ospf_database.textfsm, .*, cisco_nxos, sh[[ow]] ip o[[spf]] d[[atabase]]
 cisco_nxos_show_ip_ospf_neighbor.textfsm, .*, cisco_nxos, sh[[ow]] ip ospf nei[[ghbor]]
 cisco_nxos_show_interface_brief.textfsm, .*, cisco_nxos, sh[[ow]] int[[erface]] br[[ief]]
 cisco_nxos_show_flogi_database.textfsm, .*, cisco_nxos, sh[[ow]] fl[[ogi]] d[[atabase]]
@@ -551,14 +558,15 @@
 linux_ip_vrf_show.textfsm, .*, linux, ip v[[rf]] [[show]]
 linux_arp_-a.textfsm, .*, linux, arp -a
 
 mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm, .*, mikrotik_routeros, [[/]]ip(v6)? firewall filter print( all)? without-paging
 mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm, .*, mikrotik_routeros, [[/]]ip dhcp-server lease print without-paging
 mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm, .*, mikrotik_routeros, [[/]]ip(v6)? firewall nat print all without-paging
 mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm, .*, mikrotik_routeros, [[/]]interface ethernet monitor (\S+) once
+mikrotik_routeros_ip_firewall_address-list_print_terse.textfsm, .*, mikrotik_routeros, [[/]]ip(v6)? firewall address-list print terse
 mikrotik_routeros_snmp_community_print_without-paging.textfsm, .*, mikrotik_routeros, [[/]]snmp community print without-paging
 mikrotik_routeros_ipv6_neighbor_print_without-paging.textfsm, .*, mikrotik_routeros, [[/]]ipv6 neighbor print without-paging
 mikrotik_routeros_ip_arp_print_without-paging.textfsm, .*, mikrotik_routeros, [[/]]ip arp print without-paging
 mikrotik_routeros_system_routerboard_print.textfsm, .*, mikrotik_routeros, [[/]]system routerboard print
 mikrotik_routeros_ip_route_print_terse.textfsm, .*, mikrotik_routeros, [[/]]ip(v6)? route print terse
 
 paloalto_panos_show_running_security-policy.textfsm, .*, paloalto_panos, sh[[ow]] runn[[ing]] security[[-policy]]
```

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/juniper_junos_show_version.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/juniper_screenos_get_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/juniper_screenos_get_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/linux_ip_address_show.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/linux_ip_address_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/linux_ip_link_show.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/linux_ip_link_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/linux_ip_route_show.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/linux_ip_route_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/yamaha_show_environment.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/yamaha_show_environment.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm` & `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.3.0/pyproject.toml` & `ntc_templates-3.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntc_templates"
-version = "v3.3.0"
+version = "v3.4.0"
 description = "TextFSM Templates for Network Devices, and Python wrapper for TextFSM's CliTable."
 authors = ["Network to Code <info@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://ntc-templates.readthedocs.io"
 repository = "https://github.com/networktocode/ntc-templates"
 documentation = "https://ntc-templates.readthedocs.io"
 readme = "README.md"
```

### Comparing `ntc_templates-3.3.0/PKG-INFO` & `ntc_templates-3.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntc-templates
-Version: 3.3.0
+Version: 3.4.0
 Summary: TextFSM Templates for Network Devices, and Python wrapper for TextFSM's CliTable.
 Home-page: https://ntc-templates.readthedocs.io
 License: Apache-2.0
 Keywords: textfsm,network parsers
 Author: Network to Code
 Author-email: info@networktocode.com
 Requires-Python: >=3.7,<4.0
@@ -13,19 +13,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: test
 Requires-Dist: textfsm (>=1.1.0,<2.0.0)
 Project-URL: Documentation, https://ntc-templates.readthedocs.io
 Project-URL: Repository, https://github.com/networktocode/ntc-templates
 Description-Content-Type: text/markdown
 
 # NTC Templates
```

#### html2text {}

```diff
@@ -1,25 +1,22 @@
-Metadata-Version: 2.1 Name: ntc-templates Version: 3.3.0 Summary: TextFSM
+Metadata-Version: 2.1 Name: ntc-templates Version: 3.4.0 Summary: TextFSM
 Templates for Network Devices, and Python wrapper for TextFSM's CliTable. Home-
 page: https://ntc-templates.readthedocs.io License: Apache-2.0 Keywords:
 textfsm,network parsers Author: Network to Code Author-email:
 info@networktocode.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: test Requires-Dist: textfsm (>=1.1.0,<2.0.0) Project-URL:
-Documentation, https://ntc-templates.readthedocs.io Project-URL: Repository,
-https://github.com/networktocode/ntc-templates Description-Content-Type: text/
-markdown # NTC Templates
+Classifier: Programming Language :: Python :: 3.11 Provides-Extra: test
+Requires-Dist: textfsm (>=1.1.0,<2.0.0) Project-URL: Documentation, https://
+ntc-templates.readthedocs.io Project-URL: Repository, https://github.com/
+networktocode/ntc-templates Description-Content-Type: text/markdown # NTC
+Templates
   [https://raw.githubusercontent.com/networktocode/ntc-templates/master/docs/
                         images/icon-ntc-templates.png]
    [https://github.com/networktocode/ntc-templates/actions/workflows/ci.yml/
 badge.svg?branch=main] [https://readthedocs.org/projects/ntc-templates/badge/]
 [https://img.shields.io/pypi/v/ntc-templates] [https://img.shields.io/pypi/dm/
                                 ntc-templates]
 ## Overview Repository of TextFSM Templates for Network Devices, and Python
```

