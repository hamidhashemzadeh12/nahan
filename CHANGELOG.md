# Changelog

All notable changes to the Project Nahan (نهان) gateway will be documented in this file.

---

## [2.5.6] - 2026-06-18
### Added
- **Multi-Proxy IP Load Balancing**: Added support for multi-proxy IPs delimited by commas, semicolons, or newlines in both the subscription panel profile settings and backend config structures. These IPs are automatically distributed and rotated evenly across all generated subscription client configurations to maximize bypassing performance.
- **Accurate Location & Flag Matching**: Implemented real-time resolving of the correct country flag matching the active proxy IP utilized, ensuring subscriptions display correct flag icons corresponding to the edge proxy nodes instead of defaulting to a static IP or clean IP flag.

### Fixed
- **Websocket Transport Formats**: Rectified Vless and Trojan outbound transport formatting inconsistencies in generated Clash / Sing-Box formats to ensure proper client connectivity.
- **Flag Pre-fetching Cache**: Standardized clean IP and proxy IP resolving boundaries to resolve the proxy IP cache issues during initial loading.
