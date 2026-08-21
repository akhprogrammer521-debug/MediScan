# mediScan Admin Backend

Backend API for mediScan Admin System.

## Setup

1. Install dependencies:
```bash
npm install
```

2. Create `.env` file:
```env
DATABASE_URL="mysql://user:password@localhost:3306/mediscan_db"
JWT_SECRET="your-secret-key-change-this-in-production"
JWT_EXPIRES_IN="7d"
PORT=3000
```

3. Generate Prisma Client:
```bash
npm run prisma:generate
```

4. Run migrations:
```bash
npm run prisma:migrate
```

5. Start development server:
```bash
npm run dev
```

## Scripts

- `npm run dev` - Start development server with hot reload
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run prisma:generate` - Generate Prisma Client
- `npm run prisma:migrate` - Run database migrations
- `npm run prisma:studio` - Open Prisma Studio

## API Endpoints

### Auth
- `POST /api/auth/admin/login` - Admin login

