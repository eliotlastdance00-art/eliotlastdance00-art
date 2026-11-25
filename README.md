<div align="center">
  <img src="./assets/hero-backend.svg" alt="Eliot — Backend Systems Engineer (Python, FastAPI, PostgreSQL, Rust)" width="100%" />
</div>

### Production & Architectural Codebases

<table width="100%" border="0" cellspacing="0" cellpadding="0">
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/eliotlastdance00-art/super-wallet">
        <img src="./assets/card-super-wallet.svg" alt="super-wallet — Python PostgreSQL Fintech Backend" width="100%" />
      </a>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/eliotlastdance00-art/University_system/tree/main/app">
        <img src="./assets/card-university-system.svg" alt="University_system/app — Python MySQL Modular Monolith" width="100%" />
      </a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/eliotlastdance00-art/auto-bilet/tree/main/crates/railway_core">
        <img src="./assets/card-railway-core.svg" alt="auto-bilet/crates/railway_core — Rust Tokio Engine" width="100%" />
      </a>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/eliotlastdance00-art/turkmen_voice/tree/main/backend">
        <img src="./assets/card-turkmen-voice.svg" alt="turkmen_voice/backend — Clean Architecture FastAPI & SQLite" width="100%" />
      </a>
    </td>
  </tr>
</table>

---

### How I Engineer Backends

| Problem Area | Approach & Guarantees | Proof in Code |
|---|---|---|
| **Data & SQL** | No ORM magic. Explicit SQL, parameterized queries, schema migrations, integer minor units for money, connection pooling. | [`super-wallet/migrations`](https://github.com/eliotlastdance00-art/super-wallet/tree/main/migrations) · [`asyncpg` database layer](https://github.com/eliotlastdance00-art/super-wallet/blob/main/app/core/database.py) |
| **Auth & Security** | Argon2id hashing, TOTP 2FA, refresh-token rotation, brute-force lockout, RBAC guards, signed QR tokens, immutable audit logs. | [`super-wallet/app/users`](https://github.com/eliotlastdance00-art/super-wallet/tree/main/app/users) · [`University_system/app/auth`](https://github.com/eliotlastdance00-art/University_system/tree/main/app/auth) |
| **Reliability & Async** | Transactional outbox worker, Redis Streams, background workers, adaptive rate-limit governors, deterministic state machines. | [`super-wallet/app/core/outbox.py`](https://github.com/eliotlastdance00-art/super-wallet/blob/main/app/core/outbox.py) · [`railway_core/src/task_engine.rs`](https://github.com/eliotlastdance00-art/auto-bilet/blob/main/crates/railway_core/src/task_engine.rs) |
| **Testing & Delivery** | Clean repository/service boundaries so business logic tests cleanly; Dockerized builds and GitHub Actions CI gates. | [`turkmen_voice/backend` (38 tests)](https://github.com/eliotlastdance00-art/turkmen_voice/tree/main/backend) · [`auto-bilet` Rust CI](https://github.com/eliotlastdance00-art/auto-bilet/tree/main/.github/workflows) |

---

**Looking for:** Backend Engineer roles (`Python` · `FastAPI` · `PostgreSQL` · `Rust`) · [`@eliotlastdance00-art`](https://github.com/eliotlastdance00-art)
