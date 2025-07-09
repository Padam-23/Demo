## 🔧 How To Setup Things

---

### 1. Install Dependencies

Run the following command in your terminal:

```bash
npm install
```

```bash
MONGO_URI=mongodb+srv://<username>:<password>@cluster01.clagshx.mongodb.net/?retryWrites=true&w=majority&appName=Cluster01
PORT=5000
NODE_ENV=development
```

### 3. Enable Network Access in MongoDB Atlas

After creating your cluster and getting your connection string, follow these steps:

1. Go to your MongoDB Atlas **Dashboard**.
2. Navigate to **Network Access** under the **Security** section in the left sidebar.
3. Click on **"Add IP Address"**.
4. Select **"Allow Access from Anywhere"** (adds `0.0.0.0/0`).

-    > 🔒 For development only. For production, whitelist specific IPs.

5. Click **Confirm**.

-    > ⚠️ Without this step, your backend won't be able to connect to your MongoDB cluster.
