# PromoProxy — Keyless Remote MCP Server & Free Proxy List API

[![Live Gateway](https://img.shields.io/badge/Gateway-proxy.promo2you.com-10b981)](https://proxy.promo2you.com)
[![Remote MCP](https://img.shields.io/badge/MCP-proxy.promo2you.com%2Fmcp-06b6d4)](https://proxy.promo2you.com/mcp)
[![Residential Lite](https://img.shields.io/badge/Residential_Lite-$0.44%2FGB-22c55e)](https://proxy.promo2you.com/pricing)
[![Telegram Bot](https://img.shields.io/badge/Telegram-@Promo2ProxyBot-38bdf8)](https://t.me/Promo2ProxyBot)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

Official keyless **Remote Model Context Protocol (MCP) Server** and public proxy utility API for **Claude Desktop, Cursor, Windsurf, VS Code, and OpenAI Agents**, powered by [PromoProxy (`https://proxy.promo2you.com`)](https://proxy.promo2you.com).

## 1. Quick Connect (Keyless Remote MCP Server)

No API key or local installation required. Add the remote endpoint directly to your MCP client (`claude_desktop_config.json` or `.cursor/mcp.json`):

```json
{
  "mcpServers": {
    "promoproxy": {
      "url": "https://proxy.promo2you.com/mcp"
    }
  }
}
```

### Exposed MCP Tools
- `get_proxy_pricing`: Returns live USD per-GB pricing across Residential Lite ($0.44/GB), Residential Premium ($1.29/GB), ISP Rotating ($0.85/GB), Datacenter IPv4 ($0.48/GB), Datacenter IPv6 ($0.13/GB), and 4G/5G Mobile ($1.68/GB).
- `get_free_proxy_list`: Fetches live tested HTTP/SOCKS5 public proxies and gateway syntax examples.
- `lookup_ip_asn`: Inspects geolocation, ISP, Autonomous System Number (ASN), and residential vs datacenter classification for any IP.

## 2. Keyless Public CORS APIs

```bash
# Fetch live public proxy pool (JSON)
curl -s https://proxy.promo2you.com/api/proxy-list

# Inspect IP geolocation & ASN
curl -s https://proxy.promo2you.com/api/ip
```

## 3. Production No-KYC Proxy Infrastructure (Traffic Never Expires)

Upgrade to private high-trust proxy pools at [https://proxy.promo2you.com](https://proxy.promo2you.com) or via Telegram [@Promo2ProxyBot](https://t.me/Promo2ProxyBot):
- **Residential Lite**: **$0.44 / GB** (70M+ household IPs across 195 countries)
- **Residential Premium**: **$1.29 / GB** (City, State, ASN & 24h Sticky Sessions)
- **ISP Rotating**: **$0.85 / GB** (Residential ASN on 1 Gbps datacenter fiber)
- **Datacenter IPv4**: **$0.48 / GB** | **Datacenter IPv6**: **$0.13 / GB**
- **4G/5G Mobile Carrier**: **$1.68 / GB**
- **Minimum Crypto Deposit**: **$3 USD** (USDT, BTC, XMR, SOL, LTC, ETH) — **Bandwidth Never Expires**.
