FROM posthog/posthog:latest-release

ARG DATABASE_URL
ARG POSTHOG_REDIS_HOST
ARG POSTHOG_REDIS_PORT

ENV DATABASE_URL=$DATABASE_URL
ENV REDIS_URL="redis://$POSTHOG_REDIS_HOST:$POSTHOG_REDIS_PORT"

CMD ["./bin/plugin-server"]
