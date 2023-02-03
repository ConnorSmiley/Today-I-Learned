__Commands__


model Post {
id            Int      @id @default(autoincrement())
title         String
code          String   @db.Text
language      String
totallikes    Int      @default(0)
totalcomments Int      @default(0)
createdAt     DateTime @default(now())
updatedAT     DateTime @updatedAt
}


model Attachment {
id           String     @id @default(cuid())
filename     String
assignment   Assignment @relation(fields: [assignmentId], reference: [id])
assignmentId String
}

model Assignment {
id          String       @id @defaulf(cuid())
number      Int          @default(autoincrement)
name        String
description String
attachments Attachment[]
dueDate     String       @default("2022-09-30T00:00:002")
classroom   Classroom    @relation(fields: [classroomId], references: [id])
classroomId String
submissions Submission[]
}


