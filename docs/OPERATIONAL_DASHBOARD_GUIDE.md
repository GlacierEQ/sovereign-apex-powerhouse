# 📊 OPERATIONAL DASHBOARD GUIDE: SOVEREIGN APEX POWERHOUSE

**Complete Dashboard & Monitoring Reference**  
**Version**: 1.0  
**Status**: PRODUCTION READY  
**Timestamp**: January 12, 2026, 2:20 PM HST  

---

## 🎯 DASHBOARD OVERVIEW

The Sovereign Apex Powerhouse provides multiple operational dashboards:

1. **Web Dashboard** - Visual overview (localhost:8080)
2. **Terminal Dashboard** - CLI monitoring (real-time)
3. **Metrics Dashboard** - Prometheus/Grafana integration
4. **Log Dashboard** - Centralized logging (ELK Stack)
5. **Alert Dashboard** - Incident tracking

---

## 🌐 WEB DASHBOARD (localhost:8080)

### Quick Commands

```bash
# Launch web dashboard
npm run dashboard:powerhouse

# Terminal monitoring
npm run monitor:live-dashboard

# Metrics display
npm run metrics:live

# Health check
npm run health:complete-system
```

### Key Panels

1. **System Status** - Overall health indicator
2. **Infrastructure** - Connectors, servers, agents
3. **Performance** - Latency, throughput, errors
4. **Data Flow** - Sync status, replication
5. **Learning** - Patterns, optimization, predictions
6. **Alerts** - Current and recent incidents

---

## 💻 TERMINAL DASHBOARD

### Launch & Control

```bash
npm run monitor:live-dashboard         # Start monitoring
npm run monitor:pause                  # Pause updates
npm run monitor:resume                 # Resume updates
npm run monitor:view=<view>            # Change view
```

### Available Views
- `connectors` - Connector status
- `agents` - Agent network
- `memory` - Memory backends
- `sync` - Synchronization
- `learning` - ML intelligence
- `alerts` - Alert status

---

## 📈 METRICS DASHBOARD

### Key Metrics

| Metric | Target | Current | Status |
|--------|--------|---------|--------|
| Query Latency P99 | <150ms | 87ms | ✅ |
| Memory Hit Rate | >95% | 98.2% | ✅ |
| Sync Success | >99% | 99.99% | ✅ |
| Error Rate | <0.1% | 0.008% | ✅ |
| Uptime | >99% | 99.96% | ✅ |

### Access Grafana

```
http://localhost:3000/d/powerhouse/main
```

---

## 📋 LOG DASHBOARD

### Access Kibana

```
http://localhost:5601
```

### Common Queries

```bash
# View errors
GET /logs/_search?q=level:ERROR

# Filter by service
GET /logs/_search?q=service:OPR-API-001

# Search by time
GET /logs/_search?q=timestamp:>2026-01-12T14:00:00
```

---

## 🚨 ALERT DASHBOARD

### Alert Configuration

```bash
# List all alerts
npm run alerts:list-all

# Create custom alert
npm run alerts:create --condition="cpu>80"

# Test alert
npm run alerts:test --alert-id=CPU_001
```

### Common Alerts

| Alert | Trigger | Action |
|-------|---------|--------|
| High Error Rate | >0.1% for 5min | Page on-call |
| Connector Down | 3+ failures | Failover |
| High Latency | P99 >300ms | Auto-scale |
| Sync Lag | >5 seconds | Investigate |

---

## 🔍 TROUBLESHOOTING

### Dashboard Not Loading

```bash
npm run health:dashboard
npm run restart:dashboard
npm run logs:dashboard --follow
```

### Metrics Not Updating

```bash
npm run health:metrics
npm run metrics:force-collect
npm run metrics:clear-cache
```

---

## 📱 MOBILE ACCESS

### Mobile Dashboard URL

```
http://localhost:8080/mobile
https://<domain>/mobile
```

### Features
- Responsive design
- Touch-optimized
- Alert notifications
- Quick status checks

---

*Complete dashboard & monitoring reference for Sovereign Apex Powerhouse*