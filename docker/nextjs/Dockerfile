FROM node:gallium-alpine

RUN npx create-next-app@latest \
    next \
    --ts --tailwind --use-yarn --eslint --app --src-dir --import-alias @\
    && cd next

WORKDIR /next

ENTRYPOINT [ "yarn", "dev" ]