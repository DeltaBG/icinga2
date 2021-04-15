# TODO

## General - nagios-plugins-all

- [x] **native:** check_ping
- [x] **plugin_dummy:** check_dummy - Disabled by default. `force_enable_plugin_dummy: yes` to enable this plugin.
- [x] **plugin_users:** check_users - `./check_users -w 4 -c 5`
- [x] **plugin_disk:** check_disk - `./check_disk -w 16% -c 15%`
- [x] **plugin_load:** check_load - `./check_load -w 75 -c 85`
- [x] **plugin_procs:**
  - [x] check_zombie_procs - `./check_procs -w 5 -c 10 -s Z`
  - [x] check_total_procs - `./check_procs -w 140 -c 150`
- [x] **plugin_swap:** check_swap - https://www.monitoring-plugins.org/doc/man/check_swap.html

## General - Additional

- [x] **plugin_uptime:** check_uptime - `./check_uptime`
- [x] **plugin_cpu:** check.py command cpu
- [x] **plugin_memory:** check.py command memory
- [ ] **plugin_conntrack:** check_conntrack.sh - https://raw.githubusercontent.com/bdossantos/nagios-plugins/master/check_conntrack.sh

## Hardware checks
- [X] **plugin_smart:** check_smart.pl - https://raw.githubusercontent.com/Napsty/check_smart/master/check_smart.pl require `smartmontools`
- [x] **plugin_iostat:** check_iostat
- [x] **plugin_raid:** check_raid - https://github.com/glensc/nagios-plugin-check_raid
- [ ] **plugin_ipmi:** https://www.thomas-krenn.com/en/wiki/IPMI_Sensor_Monitoring_Plugin_setup
- [x] **plugin_snmp:**
  - [x] check_snmp_netint.pl - https://exchange.nagios.org/directory/Plugins/Network-Protocols/SNMP/Advanced-Network-Interface-Check--2D-check_netint--2F-check_snmp_netint/details
  - [x] check_snmp_mem.pl - https://exchange.nagios.org/directory/Plugins/Operating-Systems/Linux/check_snmp_mem/details
- [ ] **plugin_bonding:** check_linux_bonding - https://exchange.nagios.org/directory/Plugins/Operating-Systems/Linux/check_linux_bonding/details
- [ ] **plugin_sensors:** https://github.com/matteocorti/check_lm_sensors
  - [ ] check_cpu_temp
  - [ ] check_sys_temp

## Service checks - nagios-plugins-all

- [ ] **plugin_http:** - check_http
- [ ] **plugin_mailq:** - check_mailq
- [ ] **plugin_mysql:**
  - [ ] check_mysql
  - [ ] check_mysql_health - https://labs.consol.de/nagios/check_mysql_health/
- [ ] **plugin_smtp:** - check_smtp

## Service checks - Additional

- [ ] **plugin_docker:** check_docker - https://github.com/elacheche/docker_check
- [ ] **plugin_fail2ban:** - check_fail2ban.sh - https://raw.githubusercontent.com/zevilz/NagiosFail2banStatus/master/check_fail2ban.sh
- [ ] **plugin_iptables:** - check_iptables_status.sh - https://exchange.nagios.org/components/com_mtree/attachment.php?link_id=2437&cf_id=30
- [ ] **plugin_chrony:** - check_chrony.py - https://raw.githubusercontent.com/melmorabity/nagios-plugin-chrony/master/check_chrony.py require `pynag`
- [ ] **plugin_memcached:** - check_memcached.pl - https://raw.githubusercontent.com/willixix/WL-NagiosPlugins/master/check_memcached.pl require `perl-Cache-Memcached`
- [ ] **plugin_redis:** - check_redis.pl - https://raw.githubusercontent.com/willixix/WL-NagiosPlugins/master/check_redis.pl require `perl-Redis`
- [ ] **plugin_rbl:** check_rbl - https://github.com/matteocorti/check_rbl

- [ ] **plugin_???:** - check_service.sh - https://raw.githubusercontent.com/jonschipp/nagios-plugins/master/check_service.sh

## Cloud checks
- [ ] Check process
  - [ ] Docker
  - [ ] Nova
  - ...
- [ ]
